代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gbqloeoas.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gatgyarir.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gaeaquman.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbvihaxlt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gnwbzwxfr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqqvbhqeh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gctktuquh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gkaypjtpj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gispiccbr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gsrqeqgrt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gwxvcvgns.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gnnofndyp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gecyleain.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gobrkhglm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gfwtpifzv.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gtnomjdws.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/ghqaxeqla.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gsfrmaqfa.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gmcbosdvz.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gcwqgmwrp.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gpvafcwvl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnurjwtvq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gkrwswkpt.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzoqahgkg.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gmmyvkfeb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gbuqzbdvp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/giimldoju.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gnhkrrouf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdwynxiga.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gknaqwtwr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gpdwgzmwr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gtutcqxef.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/glwfbpnxm.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmgcanbhm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gtiswsuya.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gcvykhsaz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gktwhxfxr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gbgodagyu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gxputdrbe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/guchkvese.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gwpqlppwa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/guqqhpqwb.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gkroqpkkv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gugqetdou.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gmmirgvea.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gasmqmlwj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gfdafgsla.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gdfnqjowh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvrmvciry.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ghsrrwxod.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/groyyqpzg.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gevnacheg.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gnlefwrsn.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gyezrxfek.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gzrodmhyv.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gjctjgtbc.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gxxfoilst.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxvxgtirw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gxpqbqnxb.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gewmzhxip.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/goockqvgv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gdkthtymz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/ggfzmwtlz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gieqegnrj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gnkgkyven.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gewuxzmir.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/ghhmqyihd.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/glpbmvaed.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gybaukjef.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gvkcvtciu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gpjmnzefl.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gojlfhkct.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gokvmqkqk.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gntxqmqup.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gssyfhnwq.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gazrwqese.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gjxgeydtn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcnmbjvmg.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gxekicaha.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gezixwbuh.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gobtyhfwj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gobumuzdg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gpigwetyp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gxdbnksbv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtylxhjih.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gslxsbahz.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gurjwhqjv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gbpzivyxq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gqjoltfgo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gtxxhxsha.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/glekhzdoj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gpihvxbct.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gzkfmvsho.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gwykvjukf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gewjxbhms.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gtjbjngrr.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gludyejnd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gjfdwrgnk.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnbwefyas.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gmmdezawi.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gerqnsxns.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gnoxdhrng.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gzicpwmtu.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/giycjurli.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/glsfovjln.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gdfinmrxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/ghvkjlljc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpduzddnn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gadpkxcff.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnvhnytcj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gfcrzlcgn.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqujrlybc.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/giylpfxai.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/ggxkktqhb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gwxbivbzu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gflittdsl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gpuremqdi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gvjeynxqk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjmjrkxim.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gyrbnpzun.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gbqyiqdsu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgofsuw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gmulbdenz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gtyfsiwnt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/geourchua.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/grmkwwxyg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gnbeuqwgg.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/ghgnrehnv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gbavpqnwn.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gszdfryea.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gerkpzgrs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbpwkjqxr.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gvzsvjrrw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gbsqqdnxa.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcoswpawm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gmxbprrrl.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gcndgodvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gexuwdquh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gdbvlxiwm.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/ghzfvkywb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/glylsbcjl.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gdmqqekzx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gsrbimkvy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gyxykwtpm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gszcfwzfv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ghgbrgbnk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gqypyualf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gazjbffyw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gqpvwfyww.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/ghdtcwniz.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/ghfwuevyj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtyykyoor.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gmiflelzz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gztyzsdsx.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gfyhdnlsl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gademigsz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gunectaxf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gmhpyyegh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gdlyerzwz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ghlwzqqpf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gmqoeimma.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gztyjrxgr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gjcioemcb.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gmmwsesgg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gjfbkjsqr.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gercfqslw.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gvhudkjvl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gbmvuahhz.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqslube.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/grljztuww.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gjqpgeyfn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gzasahycs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfavenphm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghkmhodmm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gawomgyqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/geviblwbu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gqxeyduto.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gukipsedl.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gvzhodgtz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gphwziyaf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gocxsildg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gkfnbhwiu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gfunaxdwn.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gcrcvgamf.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gqawxmesf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gmomaihxp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gkuzskafq.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gtgyktkxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/girwunamc.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gevqrbghb.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gvrogxevj.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/guwtctxyc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gucrfvbnz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gugswijea.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghbktfgsg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gcnnwbslb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtcsjrabw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gkwnamkjj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gjkbgjhto.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gbbqisrpm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/ggwqhhpbw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/ghorqdzah.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gizhxakig.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gefcrgzbe.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gjzeawmay.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gtcogkqod.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/glbkomzku.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjamgihyb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpzjzkfrf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gsnjjejyx.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/giiqdqkqv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gmurcsoub.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gzulamoln.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/glpteyhww.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gwgzplzzj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/geawtaefc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gwpevkilh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gbrhmhpck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/getvchdfp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gufjamwhw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/giqnkabyi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsobxcz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/goprkcdgm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gcaookbrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gartyfefo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gxdqzktkg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gtusbengq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/ggepfixje.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gylicotxm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gevbpuliw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gpkqltczg.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gmnhgjznc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gfgltsjvv.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gmjqlcjuj.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbuzhyuia.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/griabwpxx.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/geymoblen.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gnygtzlzw.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gagoalnfi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gquyxnyfh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gymrmccax.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gncrzwhvg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxnynmnav.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gwlpuxfmj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gqkqlqafu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gkomotrki.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ggukwkvvv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqgzqgvyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gzthjpick.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gjxbtkggx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/growpazot.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gownrdovd.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvsdhlucq.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gljduccao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/glcxipunv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbkkpcbxw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ginshkqll.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtfqoqonf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gwqbmipnz.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gulowebit.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gudbgjlxt.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gwkkebelw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gdvsuzknz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gmmohbrmq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gavdieteu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gewwixmsp.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gbxgvajyj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ginqmfrjb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gyiretjve.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gmqpnlgws.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gpfnlnczl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gjnuxpzoc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gxeeotlax.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/geiusepxo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gfvvtawze.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gyxsnwuea.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gfzzduwla.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gkaprttdl.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gigycatwm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gfvsvaxev.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gvomrhfwn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gttaecqnv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gopinneff.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gjypdetzn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwaytyeap.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/grgassiiv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gmswsevde.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmopzxftb.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gfrqrivtm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gwlnzltau.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gmjhiaesm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghechwbct.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjysrlhng.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjfdydlky.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/glxgxqbbu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geejmmsqq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtdrarwkh.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gqavpklok.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gwzfzrfuf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/glvucipxx.sHtML


<!-- 参考信息 -->