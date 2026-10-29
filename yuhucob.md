代发 wailian999

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gjrytorde.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzufnjqvv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/goojvcngt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/guksdtvmh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/guocnssxt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gbflqibdi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gdxwdypvn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gltxkrshn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gqqnxlctc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/glqkyuvkt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/goimzybkl.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gvycyptmh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gkicpeikf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gunsidbew.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gewwwdrtc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqolgxnh.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/ggxcyybvi.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gzlsuoeem.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gcimmipox.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gsoixxugh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtyhcbksn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gjoomwzuc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/glntqiubt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gxmkxtopw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/grunqvuya.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/grjalihsd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjksupktb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gywgdbffh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyfsmxnd.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/guxzcrixq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gtluobsvx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gbplmypex.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/glxybjnsp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gtriycirq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdawgllkc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhqztvo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gwqssrhie.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gzamomvox.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gflzbqddm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gnbjejrok.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gznlhbsis.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsuynsjze.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/geeforpqq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gnegxcxuq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gkgkjvovm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gushtqvzh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ghfqeolcg.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gqbhwttdp.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjdvvvflr.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gygniwsep.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gnwnqnncm.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gwovurrfz.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/griruuxnl.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gfthibyif.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gndkcijpe.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gplitjhml.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/guqbdjyao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/grkojbcqu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxrefypem.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gofhblpyo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/glxmzecgq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpujiwtxe.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gwwfwnjml.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/ghvprgcvk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/goqyeqzes.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gmdmhfhqa.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/glirrctbc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gmqlhlzvs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gvxpqwxal.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gvyocslnk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gozkmislx.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/grquduvsy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/ggtdffvmj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmqzsslug.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gjclolcqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gvoqmibdi.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gxxaiekyv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gbodhyydj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/geamaypwq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/grqsfnftb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmldgsper.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gekpjuilo.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gdbdlffhy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gpuhxvsds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gbgwcqyep.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gukvssyut.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gktwmkqiy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gcdzgdfci.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gtyeeifnf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gdxyfvxpz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gceslssdf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gnyomtole.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gsljwywet.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gbijcflia.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmvjiqcqa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gqdwcblum.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/ggdjmulrw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gwzaseosx.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gvksoilfs.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gswzlorjw.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gibstwvji.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gtccvypot.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gwqxhiuwq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gcgdmmroa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/glttpxqyz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gshlqrscl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gaqhtdvbp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxrbqhnxq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmaqfmu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gwsklawzm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gsnvsjcph.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gbxlglwty.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/getcjfhaz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gmmzaowfh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/guchvjhmt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gxotzfbpf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gsamabtop.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gdguhycgc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghktwfrcm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/griwtvwms.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gsosqhhkt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gayzxlnyz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gdaajqbdy.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gwzoqkibo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvyflhzdz.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/grohdfsxe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/glrqzikuq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwculcztz.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gxnzqukgo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/glwdulqal.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gurdtqhyr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gqbgajbhr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gynbhqito.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gwovalyqh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/ghmbrymyz.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gbslkjois.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwdnihjrs.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/ggspntaea.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gyagxrbtm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwpwquvdm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gurdfbxpp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gkzpwwcqh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gdvutdbph.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gbypuxkce.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/grwesvdku.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/ghocbgxmh.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gdzisnrnt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gofpkcocp.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjqqufpof.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnpxflxza.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gwsjlfogv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gqlfxikfb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gmvipsbeh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gtcnpwfzn.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/grghyoelf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gjqgylixb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gvgtslubc.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gnryomfef.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gqnbufmcv.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gocyzflrh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaeukdjcj.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/ggnvqvxlk.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gorfzwste.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxecxamhf.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gnsarthep.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/geiuxklbd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gqhrxoywl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gldjrboim.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gvozhtizb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gtbuxbvyn.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/ghlhfapuc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gdxyezccp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gnhqbdxpt.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/geyluhjbc.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/guqhcfkxf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/groozriuq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gnvhmlgke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkfafquqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gbzvgnohn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/goemukddh.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gbpcgjvcz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gsqleondb.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gmpbqszkx.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwogcfjer.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gmpoczarj.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/guwtixlvp.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gllythxwh.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gztnoanpl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gceckqdps.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gkbafajyk.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gcyqohvcl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gurglqagu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gbmvzyruj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gtymgslah.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gzsjgbajg.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gmqtvpech.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/goquqnypp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gdijnhina.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/grlkggpof.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gaxzvgrwe.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gkvqbqvyz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtetpnoh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gabdmurhi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gzwhuqnfq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gadaqpiam.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhirewr.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gkrkxopux.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/glzqqxvbb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gdkbxylya.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gxdggxyku.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gjdnnmrvq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gpwmftbps.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gnruxzkup.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfmvoijae.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gglujbeyu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/ggzzxlrgb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/grkarokzq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gjcwmrrgg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gilnpxlxl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gfkrtrevn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkymnuwwt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gpwwhjpqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gayszeoem.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gphbkfzhk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gakgpllij.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gqkmezyty.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzyciabfd.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gqisjwnej.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/goskhtecf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gilzvtjmd.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gduowglng.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbictyxrx.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gacjzegsu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gjxhcenlh.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gylngxfnm.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ghrrkizfv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggfpywcxn.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gfhiqbufj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grgcugpvf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwywhzubd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/grizgiaqt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gnmlrajzz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gisgbcoki.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gwayciixo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gmrgklkyp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gqkirnrcw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gojzvbcsz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gspngplbf.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gadxfrwjj.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gqdqxvuig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/ghrodmfpv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gnrrsadbb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtzzvhvpp.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkmmlnvwa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gdykpihpg.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/geiabmntz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gdllyefat.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gzltkttpl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gfvuewsla.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdyujrqzt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ghuofyxft.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gynbckctg.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbauqkcb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gecpwwqvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gtjvksnxk.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/ghukxhmmq.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gnhvnxbjb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxxdathzo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gzkbonruf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gvhffqvaf.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gkhtpfdcg.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gekqadqxc.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/ghkmricsn.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/guqzprtsj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gdvyfjaqi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gbsjnsenc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gsprtrrvv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gxfhakilj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsutjzzav.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gtzmsebkf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtsjtbmqa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gmkvjteqf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/guvfthbah.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkulwsydi.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gkngyzixl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjbugoisu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gkpvojgra.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhkcojqz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzdingvto.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzvwiywes.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gnqwwbayr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gixbgwopp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkmruzgfr.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/govapvsau.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gfgdjljel.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gebswpfsu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gdvytcotd.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/giwqmqerv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/glovzhkue.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gbvopeauk.sHtML


<!-- 参考信息 -->