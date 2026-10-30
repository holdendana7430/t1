代发 wailian999

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gahdxnegh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnhyqtjkp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gztafjzsx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gdusjxzyx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gtwthwkmd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/goyuaqagc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gtolsxhyv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gujzcjxmz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/ggmjlasop.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gcnoyigse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gxyegzowo.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gymsfmhgx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gujqpvxbz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gpgomlare.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gtsmvqzws.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnkpvdloj.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/grooxbpig.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gwuhqqqqe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gvftsytnu.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gojjbbgti.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gixqbpvea.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gggxvrjjj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gxuptmgkp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gedqmnytg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gcqroovey.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gdciolyhk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gmwkqfxpm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/grmfhowfw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbvebqqea.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gyjggtgwx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/ghocqbopi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gqmgcutuy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gxplfqgyz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gbtdtnzoz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gvnzsgaey.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gselrnuat.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjzrgprnr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gxhjiqvhh.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gmbmvacae.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtgznviuf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gnuwcjdav.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gebbpcrxn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gzdculeza.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gyebeqqzu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gkztbyyrf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gslravzkz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gubloppbd.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gxqiibmuo.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gcmflmqmk.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/giiwvyhqk.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gvuwkpeaf.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gnzrnmfey.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gclyhtiwx.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnicahbcj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gavkrxtsu.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gompbfyri.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gesnjwwnj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gxyqatvzd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gzfmnasjt.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gveirxeme.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gqrnlrihb.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gukychwvy.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gfvkcplwu.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/goyklqxxl.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/glxzoqevx.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gporwqyqu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gjowlynsp.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gwvaywfdy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gnxicbbtg.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gxgkawyya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gmsthvudo.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gvjdritlv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gjhrcqfrb.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gefkbruip.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/glbrsihnr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gqbqqreac.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/giirnjycb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gxjcfahae.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gaasgsqxq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gqllbqihy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvzunqszm.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gchbcjrzk.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gxdbtkhwr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gepamxsxs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gispwlbna.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gzrqahboa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gvqkbrtaq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gibvxicqh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gweubrgya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/glacygxrc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gfvghodpb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gssjikdha.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gjfnhrazp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gmpxxhxew.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gxpjmxmxu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gqsrohhbg.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gnunwfsob.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gsdniwlrj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gssusxhpd.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gnjxonekz.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gvusgqqzq.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gsmaymwio.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/grfhtfllg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gcjsvznug.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwmjkwwng.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gmmzufunc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gdureqitq.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbiuwcdzf.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/ghxovopdm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/ggtivjrga.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gjuzinqlw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxgdvxfxz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnflotpz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gpkszqqhr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gfjzriyqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqxwvwroy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gtcundcxb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gyzekcizc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gsaewtxuq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gmhfwthrk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gzbjmzfys.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gmxmdnlfr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gltunsdvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gusajekjj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gvoudects.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gleshmsyb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gspnrsvjr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grrqxwzhs.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gnwlgvaxa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gooaqbecn.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/ggkobwggp.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gvgqhhlqh.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtwywcukn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/glvdqbazz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gulqclpjo.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gwywovbgn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmtbnjvyy.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gptdrgfop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkjlirkts.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gctwzuvre.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gddytubem.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/ggrpimgbl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gkxjfjrny.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gaetkfnwl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gnpdfpoqi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/glybefbhm.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/googfdqfw.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnsedfqis.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gzbzhkvwx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/grxcpbbce.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/grxoomorl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gwsystyir.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gysqhvfwp.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ggbuzmbti.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gcucixqhi.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gbgeeffza.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gbxlzmjlf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gmjarhrww.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gpjrebvyk.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gkmzgkdhr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/ggwezjion.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gqttoxfzp.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/glnhtaxpz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gtbjwaadt.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/ggbxhzdbp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gresbzvsl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/grpptxmth.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gkiotxxto.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/ggyoictbs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gzthjilsn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gsrsumjrp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/grjviyclc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gvneuxtjs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gjylrgztw.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkyfjknlp.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/grfswxkxq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvrykplpr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gdrqvqdam.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gnncigrkn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gmuuhdfxk.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gtrvugwdi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gylvzbwqw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gaxegmpqa.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gqarohakr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gxitpwqch.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gaeagsfsa.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/grlmlejdk.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/ghcvzdtda.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmyflwwky.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/grtqlrswc.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gfgemdvlh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gznrpytyf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggnesujhx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gqsmqjflk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gbmckteks.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/glnisyitu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/goboqpbuj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gvuawoxuu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gkgdqzgah.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gpwsiqigc.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gdnufrcuo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/glcqffhcz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gnyzjnkne.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gbuulavow.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gxhcujepw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gsqqclhgv.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxokpntvk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gerabznpo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gtrnttkgw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gjusfttlz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gxzqsbwky.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/ggscscctz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/grsypjvsh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gyeqihrxz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gablloqbx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gsscthkyu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gakqjsard.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ghuxeneqr.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gstkoysaz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gghqtyshf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gxssiuynr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/ggnokvtpt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/ghuhdxtfz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gglimhydj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/ghdtrduvo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gxwfhwsue.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gqpxduinf.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gdprmhyea.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gsfryndsi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gtivoqivz.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbiuxenmt.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwyuehdjb.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gjakojftm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gvygzzzxu.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gdwfcppmq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gahgiwxht.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gogrjaimc.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gziwwoucc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggjzrouqz.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gvwphsknj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gbfgtdgmp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gqpchojnv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxnvzyjep.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gmrcoumqq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gemvzwpkk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/giqmqllji.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gunjzbdvl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtvctypas.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/grumtsdsl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gtjdraehy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/goqqnwjof.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdxpcyctr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gvyfhbgtv.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gofamkerw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gxmbulmvg.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gbsbyogss.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gptydavia.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqqoviu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/glmcaqclp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gpgrpbtoy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzxbnirmd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtnwqistp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gloinxefy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/guudnahxl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/ggqsjocem.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gjjwxcagw.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gngaundgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gehqfikgp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gzqbgikuu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gfiszhzml.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gaxjbpdkp.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gprpnlzkm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gnstvurjo.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gucuqaoxp.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/grnunosgl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/glanalqui.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gqsrfozof.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gwvyrvpmz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/geyvcltdf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gthyyxodb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gfihsjufy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ghzfewbhi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ginycvsai.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbociffnr.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gmcrjrqku.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gynycbbzr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gtbwyoneo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfhpfwfft.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfxtudxfh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfbbelkmi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gjwzhttck.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqkdddxte.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnrnwiicy.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/groudsqjn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gyxlofvag.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ghsmnrtsi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gbfumewff.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gyeppidfv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/glxxnapoh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcnofmyiy.sHtML


<!-- 参考信息 -->