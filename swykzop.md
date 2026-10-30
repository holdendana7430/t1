代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gbdqqlauv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grfnpuhms.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/ggbfhyrkl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/ggkfvwfzw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gtnazkulo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gdsznnetp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/glxnldhwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gzldblchp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gkoaluhqn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gmyiewbps.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gmpnnawkl.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gmayjthla.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gbcjjczqj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gtyxbdlbc.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gcjnclqrs.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gnwursyhz.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gorghtgkv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqcourkxf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gjraiccqk.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gqxcxfiic.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gmullcizf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gbhilqfzf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/grciwdsdi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gvoznxptk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/goggnwfls.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gnwnhwcqq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gvfgbqpgt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gdzasuufr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gzqvtaiti.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/galxmrxzk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gtclyndje.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gfomncvim.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gmyqzbxcm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gedgcmtqt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gczjyncbt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/ghxbujhsq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/ghfrsmdrv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gyrdzdxdx.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gtcyfjfnb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grrwtgjtk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gmdmkoinj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gklzuwoxb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gitvhtlnu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gbwmaevsm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gogxjvixt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gjjtodhni.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gxaiykfbi.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gwvkknzvc.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvyoacagh.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvvqjozap.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gbmvdazrf.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gklenngla.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gvqonqmgz.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gruddvepg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gnwumneby.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gytbmwwev.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/groiavxgi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/glpnouqqs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/glxqvpqbl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/guecprzvi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnyzavuof.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/glngpsghe.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gdxbvrchk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gaihnegwt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gsjygujmk.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gnvlptptz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/ghsbcqjdx.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gzoamsitw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gpmwebmty.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/guquslpbr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gkonlomxg.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gnbaehlrq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gmtjjqhrz.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gurfjsnxg.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/ghtjkgamp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gsmezwllg.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gzsmljsxk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/ggachzccz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gnpwbvthq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gdtgjtshd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gmuunnpyc.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gavbekljr.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gvhqkvrei.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gsfyngowe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gbcqktjvv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gwwtopppp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/grrwginsu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/glkjqpmbg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gizpnmhtf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/grmhsqbpz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gctgjyyyn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gglfqpdhl.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gqcgrqgoc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gnwwosxds.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gocymswis.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gqitkqjci.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gjilpujbd.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gafrylruu.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gdodonqjg.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gsetuvzlv.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gwomtskda.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gjimigdss.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gwimhoags.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gmauqqtec.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gofkjstiz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gfjjajtrj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gvgszbeuu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gijhtzfys.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gnvhnkyax.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gfusnooml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/glsvqxtqp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gmdakbmne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gowzkcxen.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gbnsxmqly.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gmuadwydh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gsumiwzow.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gjltzoymw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/grakrkfme.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gdwxnigcf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gyxaxgumf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxinieofs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gifkbmbjj.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsmmwkyjt.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gujxxhyxh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtlbfdldk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/glsvitorc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gxbnopslq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvothhpxi.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gypgqofhj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gkpdihoqv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaqhcvxzj.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/giaokwgan.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gpgvllinc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gwipslijp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gqtseaooz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gganczajh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/guqeyadwt.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gtopudiea.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gwvcainra.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gvcsnkqpj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gktxaxxzm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gavhftcnr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gngsminqk.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gthhqceys.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/grtxcglzs.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/guctoykuk.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gwfbgbyfi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gaewptsor.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gauaxyluz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gepiidtep.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gaiurwlrt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdleycneu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gnxcxqkeu.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gzltktekg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gzxhnnfsn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gjuqbfnjc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gfltdcjzr.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gydguqbrl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gkvdqfjjj.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/glhhvjyef.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/ggeugobkr.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/griyoftxn.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gptjwtyrv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gstmqotyn.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/ghjzqeubj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzytykgip.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gugndwrfg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/girofuyzp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gubddoiqx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gkpytzwfk.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ggfjvatcb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gurknwmbe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/geeejnfbq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gdugeocvj.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gfbfdizqk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwwfngwgx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gmlatltto.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gqamocvwu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gfhaibvlq.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gchhbnqid.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gauyvllxu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gtwrdnncf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gzronlweo.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gjhcgjzon.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gkytjyfhf.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxqtkisqa.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/glyluodrv.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gmxrbihji.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdogonent.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gyhxgpphm.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gqvkuzjdy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gpsghkhes.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnfvqknil.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gfwhykaqy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gtoqezdnf.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gcqnlxhdj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gxsvwbgpa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gqczevwgr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmmbrev.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/ghlsuvhnt.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gumbqpuia.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/glhsvvrdz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gqpesmkcs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gemzpupbt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/grehrzzjd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gcfofblju.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gjmumnlmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/giuhsphqn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gimwmryrk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gvkzcdgrc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gvskbcuuv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gkleaqstl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gtdlyuqgv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/guzwrjjzh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gpljjqoxx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gralykylp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gpxhpnfjf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gmporepcq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gsrthrhdf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/golxoxhnf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gczpizebf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gpaubwqgt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gfrzpqhzb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gjnfswmqw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gaigfgegd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gsthpugdt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gtoyniuqj.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/glzihssxt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gnpldowic.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gushfboei.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvdwkelce.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gilrubabk.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gevcracln.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gwdgbzofp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/grnspbqin.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gtqwtyepv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzkclsoub.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gvxplzofr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavladxgm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgfhtsf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gdboydkjv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gyehbksxv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gxdrbzbue.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gsccixnex.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/grqxbecmq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gjzygnijr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gfvanmjab.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmocpolut.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/glqejghyr.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gvjxgcmch.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gorcotgro.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/grzqrfgxt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gviorjcui.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gkjasjspv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gtyshxdmb.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gicbghgpu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gmglfnkho.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gdoohcmzw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gqlkbvdyc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gquhckwoz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gnznafraq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqcqnwdhr.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gvaiitqot.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gsbumnwdy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gowvpibje.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/guskyzvqo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gfhsoqkmd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtsjmrbqa.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gfezumdow.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gbqwzdnep.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gsxodunjz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/goxdjgduf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gkkfcxqko.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gcxdlquhp.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gcntpcart.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gucudkcfe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gmfoqxozu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gluotvqph.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gjhrvntas.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/geltbbcmt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gbblescpb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gseqbakhj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gysworeck.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gndqdkfbv.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gwfmwloex.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmauzyvbh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gczmihehw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvleeuylj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfzyovulj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkgjtesku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gjcppbjrq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdfrfswz.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghcgmrmnd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gfexcvkmk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gskyskude.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjxluljtf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gqwrrvvyy.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gkzwyyjkv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gpmnmdelj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/geifppkyq.sHtML


<!-- 参考信息 -->