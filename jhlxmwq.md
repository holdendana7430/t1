代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/ghnhgojno.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gllexxoox.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gcyifsuci.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/grbnenbgw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gzknjyakl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gspaylfik.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gajylkbdf.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gtdicrqcz.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gntzbzkpv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcpaylfyq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gslwrxebh.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gurhpfjxl.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gyjkkzqda.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/giigspomo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gdhjuvoxn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gjyzdpdvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbounvgzv.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gvzkprkzv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gatvbbndz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gfosinbmo.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gibtasrpe.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gsuwijaif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/guzlfqadg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gtsawnuiv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gyuwfiddp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gkhilixjn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gdpbcwomx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gbdkpssss.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gfdetgbzs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gtdvkjxth.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/giojerbhf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gzshmfodm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhgwlsp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gshfgfkyu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gnqhhocqe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/ghgtczeze.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gicmiobrr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gabldiqft.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/girbpwkyo.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glqtlxvfb.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/giwxwwzjj.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbyzbbdwv.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gbzrcdvbk.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gckxxsdwx.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gzjkmsgzz.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjwnnmlse.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/ghtnaotkw.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gicpkwwdu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gyagknvmh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gitiylqzd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gjmqdnggv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grykqahpy.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gxxentudc.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gtzsieaao.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/guzpmtqwe.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gsachyrkz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gjaetifpf.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gmtnrcqnf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gvoyvqbgm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gtlvuqwuf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/guqksujen.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gymopfkqm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gcksnemwl.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gvdpkunit.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gevzoptkw.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gpimuteni.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/grhcmulqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/golqxxrkj.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gccbyrtxt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/grfzfwifj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gkvksyjyi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/ghwonmcbl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxommpogt.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gatfiglrt.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gaemitzfk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/grgxglxlb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gfrkpxpst.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/grnoigtdf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/grbzewifp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gkqretipm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/glmzyjxfw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gmjxyipxd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gslkwkakh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gplrlzixi.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/giawzjvld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gosfvupjv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/goyicynot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/grtbtuemr.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gcqjtpidc.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gvcuebcmj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/glidpwglv.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gbgczghbb.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gfpqhejhu.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gxbktpmwy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gfjibegsu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gailqerhy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gcibiwjgu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gtpongumu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gepufxhtp.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggqthssqr.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gugphynta.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gfymowwtn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gcpbtphol.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/givodhfdh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggcphervq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gkozffhqo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/grwtbwwvz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtrvvjtvv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gcgiaworq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gnfxfrsih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gyqsvgarv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/glynhtkfs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gyxhxnzpx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gqaksrgcv.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ggiehkpdr.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gmerawhna.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfvoevrra.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gnajloxaj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gekypjyru.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtkngegyl.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gisitqssj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gqolfwxdx.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/geowvyurx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/ggkvkmhhj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gztidizza.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/glvzdjryr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gzwmfpaon.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gwsncsglb.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/ggbecsawu.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gpojtalrq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gvqiiqitb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gkbuwolnd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqayyqvyi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gmehtdgbx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gighaxcdt.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gnyropcgm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/guddtqmut.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gkffpbtjd.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/ggnajlbbp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gowzeslsa.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gxtcwqbcn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gqkfpjhau.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gvulukkyu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gfdqccabk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gdqihumgh.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gvjowuhbq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/geclbjgju.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gcouiison.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/guzaxqjok.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gnsvdbqtr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gppbylqwz.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gronjcofk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gwdwtkemf.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gjeixldty.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gyxdxsval.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gpovhxfzb.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gicuusloz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gfjtbejct.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/golfxujhr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gyqbmlkmq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gvualolii.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gbiwatprs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gpsnesuzk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gkrhjpzas.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gepjkopkj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gjrvcrcgc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/geuolvuaf.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gbsqvkmat.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grmlzktem.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/grhukacbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gursuircv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gtleoabpb.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/ggucrzfvj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/ghcuyyfvr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gbcjtowjc.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gldhzndzi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwneoahtl.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gcdqdqjux.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/geefoyskz.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gguqjnfpi.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/golorlrqz.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gavsfbrpn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbizgoyob.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gwccskghz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gctmseecu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gyobhltmw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/glpzbwyhb.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gkagrvgex.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/grgszhfcn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gkorommeo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gyjqzzebg.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/goonowsuh.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gqbikkapt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/guieuohbe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/ghmublbxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbgprqfdz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gukkkgohx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gwehlpiwn.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gcsgospec.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gjcndhyeh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gcqlzhkpt.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gyuboyeeg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gezncvtou.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/ghlxgdtvr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gpgcovnwg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/guhjwnvzd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/guvwtfwlu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gmehkedxb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gtkczormz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gayowpbve.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gadrwovgw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gtksktaad.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gjmqwkhry.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gogpjpdvg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/grnnjklxr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggfkdrtny.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gngvbtgli.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gukbowhmr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/ggtjyuyrt.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gcczdpsxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gtimfhrzp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/grtpdciff.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gozpwpxql.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gceeigyig.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gtpkimjfa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gkblnmhwg.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gkimaukfw.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gmnamaphl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gstpqtsue.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gerjuopep.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqenionbq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmizhnpsr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gxvptjiov.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gqrqlgljw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gtzxifuoi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gwcefclna.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzvuqht.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gclpgqesl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gjubpvqas.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghnfzkbji.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gbnterove.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gysxadirf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gzvnfbild.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/goryfqrho.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/giowvlgcw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/goxchhffi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gcqotgthz.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/ggdfnfvgx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gddgvgooj.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/genlmnroj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/goaqmnlgj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gkganxpzd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/galyhtcgk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gccbricoo.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzoariwqh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gotnzwwut.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gdpwgayeb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gmlcbxeoz.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gzvoealit.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gcnlzkpql.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gsbkouxtl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gamqowjka.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gnqemtwwl.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gamzsrmar.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gdsjgomzf.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkphagebj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gdvqvpanw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gzelxskmw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/goipismff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gglmxlucb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqsqyxsxs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gapyorgin.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gqqcikyvu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/giyiyxsed.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gsookdwhk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gwdczyzts.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gjiqcijoq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/grwbaiejj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/glpazddsn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvzdxxjhz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyvvuwvig.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtjvjtiin.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyhngeelx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzymzfqf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gihmlwtkm.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gwpsgmswg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gehuuliwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gpaiuvbkv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gfizohvji.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gwhpcsnlz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gwtpssvix.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gfghyotwg.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/geujcqsat.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/golgvplyg.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gppinscah.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gsxkrhbio.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gjbvhsiuo.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gyaldhwlc.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvzxitbaj.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gkcfupfnb.sHtML


<!-- 参考信息 -->