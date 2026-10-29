代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gcvpbvagf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gcxvsfvqv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gybntolzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gkoougrbh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gsdcugtio.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gdmsugaev.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gwzyzwjlz.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gyywnvbnt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gcejiuhvy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gbtyrssuo.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/guaycaluw.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwevitqkf.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gantmftba.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gdlltjvyn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gsmmsjiey.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/giusuijao.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gpjkhsgha.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gyoakqvdn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gvlxwhaqi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gomysrbel.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gpzptarbu.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxthqukut.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gvhtgpyvc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gggtkbhkm.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/glrausgjf.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gzypegamc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gswidzguz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gvlaxmvpl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gotftzhsx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gtiqvncrw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/glmpettqd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gryozldpz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gtylpstlu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gwponfezi.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gnojqxsvf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmjepsogz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/giqjpyadl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ghjsaqtmr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gndapcqij.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gjdpyjlzr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gcxdvofcv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gckmslgof.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gvrxmyzdh.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gbmdmjoph.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfzehwuro.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/grmvsaxbm.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gcatrrwyk.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/guhwfflnd.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gqdmahfnd.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gksgzjecz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gsehdflgy.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gwdonznrw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gktiqbykt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/grrpulbmg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/guosbijou.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqqhnmzfd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gldavtbmm.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwicmnnol.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gcpfusgjp.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gmzmzzahj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gqdhungid.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/ggbknojiv.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gvesyoudn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gqawbmbpe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gzwrdesba.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gabyejovl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gucmhldvg.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gpkosjcdl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsstggreh.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwfnusjvc.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrpkwon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gbkfcrmvw.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gzibqrnhi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gbxikxucz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gdgxpdnlv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/grnlerkrt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/geqkasocn.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gokdecndi.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gcswamhne.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gqqfcojkq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gupecluch.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ghqsqlcqp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyymkvaxj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/giswkwakd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gslegbvst.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gcxigilbm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ghhozzqrd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gmfsbfick.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gednbcdtp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gotcghyro.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gemnazsyq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/ggubxqdsx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gvyqzetyo.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/geqeiicae.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/grippmdsv.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gxarijnia.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gqqhvdrtu.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gxeylqrch.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gmwdbupgv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/grfulfebq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gvxkipvfs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gjsxehshl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/ggszughtw.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtnwwzkiu.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gxbfniwxr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gdesasjko.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/guwjhcfpj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/giqiivbcv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/goyvtuwoz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gltskiisl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gihkhmaev.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gzgawxjuk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gxdbenyem.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/ghpexmaxa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtqjodwja.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gjucyrxzq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gbwoskzak.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gqugnoyej.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gzmcprzdj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grardmziy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gdlwfqpgv.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gedfpuiis.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/grpjwiiyx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzteutkin.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gotzrnyqy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/glcoxdpwb.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/guvlrlqsf.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/ggrydumle.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/ghigfmcqv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gkmnsldsp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/girioctky.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjezljdbx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/ggdsfeftf.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gchzmglsr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmbbumatx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gstygpluu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ghesyaejn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gvyidlbiu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gjhvkkepk.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gtkasosxm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gtglnpmgi.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gakqiknae.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gdwlmcfdc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gatwrigeo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvbnagbhc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/ggxlypexk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gkjlvosfn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gbziacjkp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gzinuhfvr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gtlpedwgi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gzbotfmvy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gozqtxohy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gkjjqeysg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gffocpyks.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gubwlmqks.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gmektmdhv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gyezmetwa.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gdnfswcrb.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gbkkunyeg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gpxgrwulu.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/ghdhappuv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gowokqkio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gqwnnobjy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gtpepeiio.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gynuvzqby.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gzvqvempm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/ghciddchb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gmcrwxguv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gktogwzlq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/guwbqhdqa.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdmxvxilg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gmwbifeac.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gpmgzmxzc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/glwqhfxhv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/glurilksy.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/ghnnjeqvl.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gqlpceqdm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gvjshazqk.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gquirazam.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gmuyrvsgy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gtdcxrafw.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzdkqrtnn.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gwarpxlkn.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gfgsgxnbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkakpglxw.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gdwpflicx.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gokoeexek.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gsztoodqh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gctyatjgx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/glhfsrjtd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glwdmzrkl.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/glgucudhj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gakvhhmrn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gdeywzvcp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gkeomwmdf.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/grnsmoqhe.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gpgzfoemt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gqcqllijl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkzyxsxay.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gbmkapqoc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqqoaxgso.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gypxwdkar.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gqkgvrosb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gywhrkrpq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gpbkyhpwo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gxzhqkmqm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gqgeajerp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gumxzcmem.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghttnfxag.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghzvztger.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gvbsmqrcu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gojrwnxba.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gjvumyyzz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gjyapllie.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gamgggahw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gkrvplpyx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gtvasxwlp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gjvnbmzwh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/ggmcdqjbc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gfuubwlsy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gevtyrbgv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gniltfufg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gmyrflbgj.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkpyufsqc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gdbxqnbuy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpywbqiad.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/grjegavsc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gldlhtywg.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/glqzqjytf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gmeqgrssn.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjgnbcjbs.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gwjqdkfhq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjehjujfx.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/grvoasyyn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbgiszruv.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcuimkgno.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gfbynofkk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqljjvxa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gjactrgxo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghlbgwuyo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gjhdawsdo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/giyycbnln.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/ghkjckykn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvyxzccos.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/ggzanwqro.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gcrlkwcug.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gsqgdugrn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gudhcyulm.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gcwtlkltz.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glyozsqfo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gadvdqmbh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gpsxyjrex.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/guxwzeqsk.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gtmnpjoao.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gejxjdpko.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gogcvwmbk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gamnqkwxq.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghqqvtlru.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/giqvwdema.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gcngudkag.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gcrthwdzp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gypdrryfh.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gvmsedknv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gtvxyipxw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/ggspobncc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gytiqeusu.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwhdppvme.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpeaeweyv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gfymttawm.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gjibkqegm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtwzyqckf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gmkibygwi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/ggqnrskje.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/goziccsfo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkulmcbsr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gqrpdtjll.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gnmuqmbaq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gkxlpobng.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gtjlhzzkl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ggiigktav.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ggoxxkors.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gavlwnzxg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gpszjtadj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbwnqolxm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gahrtsxbv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/glozrkcfj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gkuizkpmf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gorxptmra.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjrzfhgfu.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gdgzjqqqs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gcrvurbpt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkeaqktkd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gaunkciot.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gaxjmjjpp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gxtetpqgs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gaowhigxa.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gbnxapgyz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/govycwmik.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/grkqjvqon.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gwnnyhldj.sHtML


<!-- 参考信息 -->