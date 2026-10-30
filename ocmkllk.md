代发 wailian999

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gjfwtjqpz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggkotqykh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/ggwmnurgq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gogkxgcql.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gwbiisziy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/goarxksbz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gnxlvkrus.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gqrpvyvim.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gafylwjin.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gcwnhnoaa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gpyyaftfs.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gweyakkka.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gornxwgsf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gnqpkvovr.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gliplyhoy.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/glpzcvhde.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcrduihkw.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gbqoqirvt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gdfduodwe.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gsndaghzy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/geebdyyqv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwoyvsbtx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvfdfrt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gqeuiwshu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gtudciqir.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ghbgyntls.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gtcedervz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/giqwroobh.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gmmmlzqko.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gztsxosar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gxxnylwkd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbbpvyaqc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/ggxzwshbk.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gwwhivnqn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gwdfoketw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gbsycbujr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gntefssfo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gpbimikhn.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gcuenyaqy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gldsymzrf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gkbymnluf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ghtghfofi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gufkdrtvw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gozsfcfvz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gzxdczkxr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbekdaqoy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ggxwnuvkh.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gomiviocs.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gckljtpxb.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghdiatuoc.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gedhqouxj.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gnhipmnmv.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/grluhnqyu.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gvzscwirc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gjxrfyrzk.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gajbzpihh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gwoexksqi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gqbvxirgd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gmwqtugpk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdtyztjjw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gqiecstik.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gsehaujbb.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gwpmrmodp.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gekbsppuj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gzdwcrmpg.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gaozqtiac.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/ghmkopddw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gclmhhbnv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gswxafqbt.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/glbghkzkx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/glmwkbvvh.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/galwcjhcv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/giruabgjs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbbbnpalz.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gwvrilvtm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gqbggimmd.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gtsbfmonf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gkfywfnka.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gmoxkvyoj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/ggrsbqvea.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grdazgrws.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/giecdosrk.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/guwnyoxau.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/ggnpwajed.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnaketn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gnskfhlmg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gznirlzsy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gjwmityad.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gsnxpntsi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gusdqykzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gilwtsqsy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gdebyhoov.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gifvfzzoq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gfjeauxkf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gpurpznro.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gswlaitki.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gjbbvygej.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gzkuxczaw.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gwslxjwij.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gpvixjrwq.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdeyhwrjl.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gaqlguxlk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gfrzdchhe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjsxeelke.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gzkxbieyk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/guxpvopwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gfybuojhf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkimhnlpp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gquqdilom.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gmftjuxtg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gjyvpulsf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/ghmpadvwk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gyvfuqpqz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gatritfvx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsiejywo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/geeivyyhe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gcaouwgxy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/ghdbehgbm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gwwsbsceh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhrlqib.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gekvaveot.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyoluaa.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gfidtuuvq.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gxlwjaoow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gckamizfz.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/godvnvdis.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqfjsbzvk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtpytwqax.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gtophuain.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gytvpojut.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcnnsinpn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gskeqvkya.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gsccdczse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gzxajjwdw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gzkvpuflp.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gsyzrdysz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gnufippia.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gojhpqzgs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gegekhayn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbxmefbgs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gntdajwuh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gmqpcoeqc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/guhubtsvn.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gmikgifty.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gfmtgxdzf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvxvhui.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gqptmcmam.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grrvaovxw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gakelzmyt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/grflstcce.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gkzzhrcfc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gxaoaoetl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gggmfzvns.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gtlkcvfhv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gerfhayec.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gqagcsfcj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/glzztlxqi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gmgjzuidc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gxjujhmyq.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gnfhzpqgi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gsaguzjgc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gebcdscaz.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gddnkonrp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gakvflazc.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/giksfdarq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gpnqpkwrq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gjkbucaxh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gnuwgavbk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gqutzuqjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gierajrep.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gfnlgobdi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/guxgumrcj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gnifbdygb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gmsgnwkdu.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpeqjjbcv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/guurfobvf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/godmublbv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtjbanwbn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gtwfvpolq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gkwrobgqn.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gjfvqupnm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/glsvxdkfu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gqefbccqf.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gaddlsclw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geplrcbxj.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghozuiiiv.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqwjgmoay.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/grkleiqse.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guokrttee.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/ghrythqet.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjtnayunl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gkiendclm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gytcrijat.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gqqnqewvb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gddialwys.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gdsnlnzhr.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gjqysalad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gupuktltk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gxmsrqfdx.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gyhlbkuei.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gasnetfsp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gtgrycijd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/glsdplare.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/graihhpwd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gkslpcrxy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gfqukerwb.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gcrgpovtf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gifrwlcjj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gtzjjqorv.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gyuxprtnf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gzvjiedsw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/grubozvpi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gjcuaxrss.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gidjsxhfe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/guyogvkxj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gbrhlvqra.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gxzrebogw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gowznxwtp.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/ggxyrmzim.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gjaudfyed.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gpwurxxdt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gsejdhzxx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/guslyabnj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/goobbqsmg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gypsneuov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gfpinaycc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gexvtijkx.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/glzzmxrry.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/goflfyojr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyrnbtdpd.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gzeudrpnj.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gaebjdihr.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gtkuznaci.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gbipwdlkq.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtfxazgps.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gmhmncsvl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqeoyrxxo.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gvnzafyem.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzotqfosa.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxjlillky.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gaebreour.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gtnjrxoww.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gqvdlugki.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/giesvjwrt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gfuriwbgc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/grmyrjdmi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gxolpffix.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxopdgkjc.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gbsragxus.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gcxmivqtg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/ghcrqsvyg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gugtbtbuy.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzikeoupw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gmuuuxgbs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gedvdwnqq.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gonlgxxoo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gnqtefpkm.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/goptssqnq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/glhzumglb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvxubzdog.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/ghotgwasg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gktpbbwho.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gjwkyfebn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gdquckfhz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gzryjqklu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/ghhoynfxc.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gxuchurxu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gjwiylyni.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gyjpsogyn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gubrryxzm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/geqpzzydv.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gymepbooq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gqrtfwnco.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gkydjawwo.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gjlnhwode.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gqcqmzyoo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gkcqinrmc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/groxfymvt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gifyzpfug.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gdlqeqhke.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gsgkevzwb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gtohjmpir.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gkduwydck.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gilihggnu.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gxrczeasq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gebkjwtft.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gdhkmhnvm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcjgxdtnc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtpiaacud.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gezxkedwr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/glbxbkgqg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsnubxfoe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjvbyvmbf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ggtcushwn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gycunchdn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnexxyvjc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/giloslymn.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gxsezjino.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gixtyrcxp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gmftctqdi.sHtML


<!-- 参考信息 -->