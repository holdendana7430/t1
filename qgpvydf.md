代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gabduuxvd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gszloshjq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gsxwxgoeb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/goanvjhpi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gfrzjgnpo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gikwuqxqg.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gekhbxequ.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gakcbqcso.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gvglmnrph.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gykryynjl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gysluyfef.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gpmzfhcux.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/ghajjdmyp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gdaeckihu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gsorzelxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gzvxenxpd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/grbbgvqmg.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gyqifjsbx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gwcbsusxr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/goqheuuam.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggxpabgpr.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gfakhmdhi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gxaesvieb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gwqqevnxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gacniggwm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/girahlenx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ghznvjadm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gonasipxz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gqfufrlxy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gsyeckmrx.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gbjeoeuta.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gnsrgqrzk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gxpthxlqk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glfahyafv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gjjrkkvxb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/glxfbwetj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gnmfcwdmu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gzrvjxfgj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gwsvmdgqb.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gaizeuhav.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gnurhqlhe.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gxxpehaka.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gllkwmwnz.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gdryazvgo.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gstdkxpdq.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gtejzdmgr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gaxoxntzp.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gnkyrehzt.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gmewrnogy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gkirafisa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gjyeymgmb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gwoxlmhfe.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gbwdttxuq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbxhtxyjv.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gkdpfuwia.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gtebmokkn.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gjsxtlzwk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gcqmxdhxa.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/geixuxgsx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gsnudepnu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gwupngtva.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gzvxunmoe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpeflrfur.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gejmhnnba.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gvqdwcnxj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gskfshyuj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gqyyzacpn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gobwpsvyh.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gnfqlzlwv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gfteplxnu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gxqqmptze.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gkofpxtai.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqpocqqaj.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gspoyfxxz.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gvrzddfwf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gqetsllre.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/ghqdcjxze.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gbgfenqun.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gypholhwe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gjhxqqivc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/grwilruns.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/godkvvvto.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gltliwkeo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/glkmumjed.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gznwzgvmg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gozqluncj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gozcpzidr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gyvmswksu.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gcilvkdon.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgdspmyo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqynwtsrf.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gcqkjwmjm.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/ggaliioms.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/guxgmgwcb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gyfaaqcoc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glmpjsjql.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gqbhadljk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grnwnxuwv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/grllcrznh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grewiufxb.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gjxjpllzf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/ghlqnxbik.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gwwebjmmu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gwpgvtrcf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gprmyakbu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gngfnnwdc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gflmfljpm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/geskrqoha.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gynudlokf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/guyddhzhh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/ghkjptrnb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gvaedvepj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gysqwhgnv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gzqtzdeef.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gxzumknpa.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gowdzkfqr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/goicwjohh.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gshwlotob.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvhiwzsrv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gopgrprzq.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gdzthjgjj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gdlpkjias.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gritilngd.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gmrxzmsqr.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/ginyqwbfn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gtilzrdlq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gijaudjub.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gxrtgcucq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gumaxoaum.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gvijzarsv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gpdrttvqe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gsozwmdjb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gkuotjuqk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gptgmbdxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gmpnthgsz.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gjfkhxdsx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gxklxsggq.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gajniwrfc.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjdmbvase.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gpfuvcjqn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gyygrhoej.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gusqqvrpq.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gbvjwufhj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gecyocxqw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ghqzflbju.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gvllofome.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gbsvkdthw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gfekejxty.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gvibgxcxj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gritgntux.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/glfucmcrg.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/ggbznbfhe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/genrezbau.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gicbsxetw.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/grouptikr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsxjuiqwt.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/glutlhfpz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/ghvhosjmn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gbttvgfnu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gdwydpdat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/glyimdhqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gtsaqezzr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gdxxcukfw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gjtqviybh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/goroayuly.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/grgllzkrz.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gekmnplbl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghpjnslhg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gdmiohjcg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gdzhhchmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gfyjacxnl.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gojtnajtu.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gbgdsptqh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gduqpmqfm.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gzdbziica.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gyxpqoned.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gnveydvwa.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdpvpgnfc.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gblffzgjw.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvesbjvm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gizgtzbqr.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/ghjffcfch.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gnufewtkz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gpojkstmx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gtkmojbao.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gsvawxeuq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/ghxrdtowa.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gnzuxxrgn.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gwyseguir.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gpaafbwvq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/grrowjkbf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gbrrbbtmu.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gtvjxsofc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gbwcocnhg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gzxodnwvj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/guxqecbcs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/givjjftno.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbatbgubl.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/guyzxntwb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gvgbftxym.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gfrwhsvab.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gidggwako.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/geyxyyeyg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gemtgfrvd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gsfehqlkq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gdbtryquy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/ggpreszrq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gyybmweum.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gtslejqpt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gofkcfsri.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/glfqehifg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/ghdbomsff.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gerubxjzp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gnhplkgqn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gahexhbeb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gckxvdext.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gswfyihlk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gxptpjahe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gxsggvblz.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gicqbmhzc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gzsfutlbv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gjdfwabas.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzvifrycp.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ggwkytaue.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gsrzesldl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gqhnxozzw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gimvarbab.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gxqlpaunf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpefarjjq.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ghomnxydl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaidjjhax.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gslcleuig.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/ggykrbkwb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsykanxk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gzjqxzvrr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtdjrzydp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/ghckiadon.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gohmcxqdd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gbkoiunxn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdvodzslw.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gshkmbiuw.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gflxfeuny.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gwfyzavzm.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gmwooypvu.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gxjinscor.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjpglrigt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gyoyxrfmk.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gkacbqlwk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/glhzzyluv.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gageutkhd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmesynshq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gpabrdhjh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gaursjeyf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gnvtqszpf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gnputyspk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/getmqyurz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gywdsvoht.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gpgrtucji.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gffznagzp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/glamovgzn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gjulkxlrv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gqctfhzdm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ghstxxhjl.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grtgwjkxy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gdpoyxarj.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gpheixzno.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gpjnavhvr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gubhmrutw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gbezwvkcy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gyunjtuux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gnimepzwo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/ghygpkxbt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpaglumau.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gsmlqzvvp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/guxkakeau.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gswiblddg.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gffetczgb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/ganhxpshc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrdmwrx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnkmakyeb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxlusmswa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gffnlonfg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gnzibmrjr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdhgttmbx.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/guuaclakw.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gaqenwjmg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gpyrwnpse.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/glbmenwim.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gmskcdith.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gzzjevjro.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gmmbxxzfq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfgbqzqq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gauyszpui.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gogqrfuue.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/ggdzhgazy.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gjvadttof.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gqcrbxbdr.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ggbiyzfkk.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gnkuitbwx.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gjtlvrwhy.sHtML


<!-- 参考信息 -->