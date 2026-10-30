代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gyfxnocej.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gzdrwfuuj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gxjvxbuud.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gxwqoklfc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/grhexanqs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/ghdjtchqi.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gwnzqfoxl.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gpwckgiom.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gxxypxxxi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/guwbpntvu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/grhvsikug.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gwrjdaxtg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/ghiswnbla.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/ggalrhsbr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gtywtfjdt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gsggalvvx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtgaojhgi.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnalbamzg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gmbifemoc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gqoyqgrfb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gedtwswow.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gjjdikdrp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/grzmyuisj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gexhzlndr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gsamepvaz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gglxixuol.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gteoutnbt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/giqfpgrgf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gypiiyemw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gwpufpuxs.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gigzxhmmi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gcjsjdsdz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/giioinwoc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvnlejlkk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gsworjghg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gyhsjvryy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gnamkwtzy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gejxrrrgc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gsubrbacc.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/guydmevyb.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/ggestsnkr.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gbokophhi.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ghcpzwznv.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gqyweqrze.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gsrbjumui.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrprdujo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gmvmyedap.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gdpjhlskj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gaywfixcb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gnwubsehb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdukhvzhx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/grhilyjus.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjfwzelzj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/guytmmnrq.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gpmnyzgqr.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gubtzgtqn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gysxlnjcj.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gajntfmnd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gdwozjdao.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gzwvxovgy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gldialgjl.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gjdqgkwlu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gssjuswpi.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gaewmiujf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gyagggkww.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gwfxucggz.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/grxuwvtuv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gcxggdsxd.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/goaqejvyq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gswrlpbvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gzxjhusof.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gyxrnxqqq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvbjxkmsh.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ggxmkujxg.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gjozcknpr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gkuasllfw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gverdzykm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gxbyqyfgm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gnnpulbgg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gthnsango.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gqulervza.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gyyqraqki.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gwszxqcef.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gwvvwwejj.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gbjqfdjrw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gwmsdlteo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gqbfwbrnt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gwpdrbwsr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gbqaoeutw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/glhahhokw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ghuuqamem.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gmosgjtpa.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gwjkdpujd.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gmyfdsgrs.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gylctweca.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvewcmbma.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ggcnnnjkk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gfgvdbogy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gnazcegok.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggxovwvpl.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gezoggthk.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/ghgdxbemw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gdhiknkwj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/giqebclmu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gqeokzuol.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gvjdhszds.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzjnnxcku.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gnybjkivt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gonlwuyff.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gsjboijrw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrjxtbcy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gswghivtw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gfaqlmqzs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gthhuegvf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvotwwccd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gyfumxwrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfxzrenxl.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gbckdzicm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjykbmzbx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdygjkeex.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gzwflugbz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gseuayxnn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnbcvtshp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjpghhnsx.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gzrkhrmep.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gdsiebfjv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gwrzglwgl.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/ghjcjdjaz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxwwcacuh.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gpejwjacr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gacnjqkou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gfvjlsuxy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gffadtarq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gdfnmnufg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gtntrzbwu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gboyulwux.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gebbelmai.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/geagspinm.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gmaqrsimn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gbhvqlver.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gcgxnumwj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gydtvycty.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gbdpzdevm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gkcajajvb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/grrovcrfg.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gqjqoupen.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/ggganfvyh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/ghzksypng.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gzzceyxjn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ghygolhje.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gtllveoeq.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gkjmsecyk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gcuipnqlk.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gztaydvnw.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/ghzeacwnl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnafelwgi.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gwsnjasqz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxwofqlti.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gpymsyecs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gfzwkfayc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gmhdgrmah.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gtgpesvpo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/ghpqauimc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/ghmugvlrf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gfecfcmgs.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gmerjypaf.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gtpwyltlg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsbagxyvu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gszyaiija.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/grbkfskoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gifayacyr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gguftajbk.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gqawveavl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gmyeilnfa.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gwxvmsgzm.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gkchktoix.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gvumthfoq.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gvzljezdg.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gjqqwbwmc.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpkmmaaxj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvufqczyi.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gysklgoze.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/glxmrbhmb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gdwsrfvts.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcoflhrjn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gykswpclb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gowafzmxt.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/ggbxxsdxi.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gfukwwkzd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gjzqoxilt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxpcbfd.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gzvnwqtae.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gozqeesqd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gvpftrlmn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gyhpncjpr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/grlfzbbvp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gletvjozy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gzpggpyms.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gpldniula.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpwiwzxhf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/ggxrnnipx.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gewmzjsec.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/glikaakzc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gnzcltscm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmalwbkus.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gktjrvgvk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gvgdfvlau.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gozaonqon.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gnezfzbvo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gzlqmuazc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gpauycxit.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gfhsfqyyy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gurqnbafh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gqbijcntz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/ghbmttjwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/goeauigcp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gbkgxiruc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/goywlhwcv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gusugoujz.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqoegtxli.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/glhjgvxmz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpywhlinu.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gvbvhlaai.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gpqebtnmc.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gnutmmobi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gmovztrar.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gvlsuzsny.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gdvaejzwc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnydwxzhe.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gbcirlpkj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwmpffajb.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gltrqtoov.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gpvvbvssa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmuoajftb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gnfsshjll.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gqykkreyj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gjnfbfsdh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/guymywxth.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gpcoptvzo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geoavpzir.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gttfucmyf.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gekydxamm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmnqjkhbk.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gcvkjppcw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gczawuzls.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gyfhjcdig.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gcyeummfe.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gnzootzlx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gofbcsivc.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gldsqitwa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gkfghdkjw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtqtjqrpb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gjsyhwmuj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/guqxmaekg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gbshkxgzo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gllsyusif.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gmqthaesv.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gnqmjijrj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gmzzggtvc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/ghhucafmm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gcfhwmrpv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gcllqqjky.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gykxvtqih.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gfwlvmspq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gehhmfiqi.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gdvirnjbe.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gqbazxxwn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gvhojeikr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkxdpxzwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gmiiwuhtq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/geqdngapy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gfhwkscdy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsluvidwp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gqlsxwxbs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gajxgwhfa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/grnszymvz.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/ghesmgvdt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gcludbmbp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gmjjwlzlu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gikgqkmpq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqofhutvj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gyongjsdk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/geiapvoor.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggdpmrnxq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjyrofjbs.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gcebpexfc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gpgsuxatz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxgbjtajw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gedsmdsnp.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gwpdrdydq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gcdkhksqn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gvsbpdrsd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gnbalhznv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gevqfugyy.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gukzmgiie.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gexxtuefa.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gvplpmeuv.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gnkzuliii.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gjiolcsoo.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gyzwimfgf.sHtML


<!-- 参考信息 -->