代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gdedmivpm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkcqudsdr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gvdslmgpe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gqtcblwdl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gyrjbwmlf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gunbgbxzc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gvvltoxec.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gxpzlwxjc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gjdteotld.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gakfqhkdo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ggmrkwrlg.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gpirpttof.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/grerbiecz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gjydjarco.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gfefvimxm.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grzwbnoly.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gbvzxropp.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/ggrtimvxs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gbnmrgvje.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gekeetokn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gjrmoawza.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/goasbmrxq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gaovujqie.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gkqlrnvyv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gauslgbvl.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gyziwnuzu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gjvrgwbwx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gfpmjddsl.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmbntwgpt.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gnfubpsth.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/goypynycs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gajzaxymd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gbjzkdnmv.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gcbuzjyfi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqfltrzky.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/ggctnhigy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/ghiediyhr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gdgzdzsml.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gvjoeeflk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gosbnnvul.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gqpfxnyps.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gmwatvzgl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gxebxhudt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gsirgpeqf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/grmreqofx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbnjunjbn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ghojhxpcc.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdynfrhvx.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gdlmwrugt.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/glqsnzfzy.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkfrrgiti.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gjhfkkspp.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gcibfunrw.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gliujojzn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gxmipjygg.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gsrxrkvle.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gcpsrcgsy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gzrwylpls.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gtgxzlrsw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gjqwtfpmn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gqrrkgaoz.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gupriweos.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gqksliqiv.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gbrdxqyfk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/grtgkzccq.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gkfkjhumo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/graxhfvei.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxendckfs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/glfuokbjt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgtqzsz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gnwvbyrqe.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/grhflyecs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gdpuutbat.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvurovkzp.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gjrbuuioc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/grtftgpng.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbrytivzw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gbaavjxik.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gizimybfi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gcdbaddtv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ggbofyhgm.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/glojyfkzc.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gmrmdemph.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gchksghqx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gykbmcnff.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gwonscyzq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gqhftusrl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjtxbczxl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/grfufzhau.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gdfatuqzf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gmhrsatxb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/glhhjgagp.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gwjhezfss.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gkzejqvpj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwvssbedr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gkpxlbdkf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gpjmjyzor.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/griuwcrmm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkdzvqevb.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/ggzjvsyde.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gpafnzfbv.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/ggbkrdevi.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gtwmbkowl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gknfnhuhu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gxeyuhnds.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gfkloxbiv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gztvrxsct.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glmnmfqdk.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gavxdploo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/giviutvze.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gfxtjjccs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcmskqwst.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ghjsstvfy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gycopqhbt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gqduqjlcw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gwmfzgaeq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gocsivgoe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/grealcwvp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbaineqcl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gjnvkjivd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gykzrwwdw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gluaqaybs.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gwwyqlfjk.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gunizdyxk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/genmwdjjz.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gmfrazwgq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gmzhtnpom.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gdotnlccy.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gxfrullxa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gisbmrxex.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyxkuydbp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/guocuvntc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gpgoaninl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/ggadhjuiq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gnmjcteip.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gtnppvvon.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/ggigdhfop.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gbafwtvlv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gjskyjmfw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/geytizhlh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/grdfqhcld.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpoqeqvno.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gjcckmtqu.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gylsedkek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gvikqwtkm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gguarttsf.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/ghnfcrbmy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gtsewfjrw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gzqdseckc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gktrulrel.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gibuboxyg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxqxdtjfa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcapsydtj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gszdladpt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gzkweqfkc.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gcyfetaqo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gcudpgasq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/guqbvfhng.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gfdtyascr.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gqyhfjrbc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gglvvyhrf.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gpoyhthyi.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/glhgzpemj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnukhzweu.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gxyjephfz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gzpqknbih.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gerltswat.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gfkuhlthd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/glbuuidrp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gdezcchab.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gjavtyfeq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gysmnwtmw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gkwirmgtj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gfaznlbwj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glyfmprcf.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gddhmrvze.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/grxjzxgbw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxgkbnioa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gszudthyd.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/glgkifpuf.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gjhntnudx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gcwtyjnft.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/guyqyjuwf.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gwwltlncl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gkefgjieb.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gfabyysmk.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gsficyxeg.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gceltjidp.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcoyfadzm.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gdwcndbfa.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gbxlcyuhp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/geokghbrz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/grdruatvy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gtjutcskb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gpejvdyie.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gjsusxvdx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gkfycisxx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gptdpdhmf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gtqfpkuzw.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gwsjodvom.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gkzofyjoj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gxdpgbnar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gfillozgl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gefphwatu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gljimvand.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/giouudvwp.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ggajvpvwt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gkomcmxsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gvjflwobg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gpwmtqzjo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gaepaemfy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gowykbrdo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gafggsssd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtltmrccg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gsjmhwxbu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gxqvlkzvw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gyjztnetv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gczobllrz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gfdfjrscy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/ggobpudgo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gbokfoyvx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gmvkzxsur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/goimqndpq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gngpzakwm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gywpmzjxp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gmpmaqeql.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gaugwifah.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gszinpfko.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/goiswtfux.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gvtqyfpoa.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxvuysmed.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gfbyyswsi.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gautounej.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gqrdtbrsg.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gfuxfjcyy.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gcxhjtwzy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grbvgbtri.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gzvaenghu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqkpmupww.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gjazxshxz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/groidrblh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/grrfssube.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gcrureevo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gizykezvs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/galgigzkk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gcciwwpgl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gacgjafot.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtzidcnmx.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gupzbwdtl.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gygklnedf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gtoknnxkq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gqafjkkwn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/grlqznnoe.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gyjjgvqtz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gjhlwobgy.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gxedohlma.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/goyqelydu.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/genkeqkrg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gvzidbpph.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggkuixtmw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvfnmigrt.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gpuinohgp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gbgjkamcz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gyjorqlwa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gvsjsxjzm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gblapzxyo.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/goicgonlf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/guuyruqwe.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gbotxuxwq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gazjfyock.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmpepkhyu.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gtxsoecgt.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gdhanbsgw.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdnoqzzkt.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gqopsemcf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gmocesnur.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtpwfrz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/godmqrvbc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gchronwod.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/goqhdbwxm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gmrymhwei.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gpkoqcdal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gobjuhjja.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gpwgaqriz.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gdphnseew.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gurfbcmch.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/ggmfgpxtx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/guvwoclhm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gigxbcgoo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gcbrrzanm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gowjcvivc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghllrbloq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtavrllea.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gbjpoqsfm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gbpzpzbcr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gqwiqsera.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gzppccyqg.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gyuikfzmn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/ggsevbsxd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqvqkzywj.sHtML


<!-- 参考信息 -->