代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/geirjusnm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gozigvqkr.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gpjyxpfhg.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/ggjrnwilv.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gismbutse.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gckmqhuig.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/glhqfxkld.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gqxoepiri.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/grddgnmlb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gzlumtdlz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gsxybvivu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gmqdcijeg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkhjyszix.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gzhxhzrob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gunowvolt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gocdfdszi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtspshwnt.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/guvlnnzup.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gaiuxigui.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnojyubdh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gliehsxrz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gvkljrsyp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gxtdqjrrk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gzfskuelu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gtnlikcvd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gzskoatcn.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gzzfpcgrf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gungnteea.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gystxejli.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/giufpajmi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gkryscoxm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gclnnsvto.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gthtnweog.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gizwmfjla.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gowwhcxgd.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gsbsvnwwo.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gdgdvrjfb.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcxpwgehz.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gzztdinyd.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gdbmckamy.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gqubrirdj.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbnrorqsl.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gkskdjkph.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/glgbwymut.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gofhvdzzn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gqylwfkkp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gwmoiafox.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gvyebqnkq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glrczozse.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gocaceqog.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gnofkdwwm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/grsdyepkx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gmzuvvxpr.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gpawugifw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gxduwtzmq.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gxkccodke.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gqdkwowqf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ghguqgyal.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/ggawskjlc.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/ghpfkdali.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gwwfqzjqm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gdqktsfam.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gzalxjckm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghgkiscss.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/grcgprwfm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gykwcspnk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/glkofdhan.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gxcxlinov.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gujidsnnf.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gurkwjleb.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/grarromeq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gjppmhfbm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gcqeabhxf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gvuelqzii.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gkzrwaavc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gyhcwynfl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gwovhktww.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gtxwgrlnh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gxpjnwvfd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gvvvhaphv.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gigsdtqnb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/grljaovsm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gvouwnncn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gnqtmpbov.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gjllhgnuf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/giewsedim.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/ggtccjusb.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gqpxmbqkk.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gbdedirqk.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gyevzdwhv.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/guyhdsekp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/giaawhjtf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gibgxoopw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gljtkfheb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gqdgjpcrz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpmkudhqc.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gwojlkuov.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gvpxrduuo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/geetzmwtz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gzhmofxza.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gwhqjqwqa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghbduldpt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gmtrbbvsz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gdqkbmmix.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gfeixqgxo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gzwbdqkri.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsfbcsgtd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gsjnljxxs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gxonwbpmj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/ggvytsycs.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ghdmvjvvs.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gdqakyfhr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gnnftvslo.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gvtyyqvwn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grutemtec.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gsckfcesc.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gbmapvclx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gawmzahvj.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gvyokeytb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gczdezmnz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gqsrrtgwk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gaipmglfd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gqcggaibp.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gsqdphnia.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gqltridcl.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gocrinlqb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gddsbdmku.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gymtjsnbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxvblqq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmuaantpm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gxkcujvvg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gvpvykbcg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gjvpqgbeu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gewgljdlj.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gpuzvyvus.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ghsuakuhy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqjrqmytc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsypkdgc.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggpqrrrjt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gjuhhtqtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gsydogtvc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gdykuwvun.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gcxkpoybq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gcbklyvre.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gjgytyfse.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gksuestpe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/grunnobby.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gvgyrqdsd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gmiyideew.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gvhmtgabx.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/glcecylhe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gfsmrotmf.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gsuxhgugr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gdhsjwthv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gddgdthmi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gagvsulav.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gaspzgfgo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gcktkwvfn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gsfjtgdit.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gcgrgdjoo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/ghvhpwrzj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gqyltwlui.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtlladjsg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gvevafkdk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/guhrzztxt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gbphwdsnd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gnpqdniun.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/ghuxetugh.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gnrikqzjz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/guycpdjvo.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gugqzarbg.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gymhpqcwn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gtahsvjdx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gndieioaa.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gbxdvbgga.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gagdvdwoi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gglplsqpe.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gebyjgbwe.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/glpcfnrmh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gdbiwronf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjbbowugm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gyukjtiqv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gmruxnjge.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gpqwuqkhg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gsvppevlw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gyzcvfqvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gbsjnvvhh.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/goojiybln.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gxxlnozvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gcvxevkti.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gizjydmgq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/giksqahhq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcgjmcexc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gprjlidou.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gmacygfhu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gkioufujd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gwstlrbwc.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gcanxjkcp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gzvfliwog.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gifguafmm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gxrotdxkz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjzbqpvzg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gwdlxoigl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gyckemsue.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gkykbipkc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gxxhxzmqq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gueptwbax.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gziphbhbn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gpzdqnrws.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gqukwnsyb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gijshefog.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gkvqyylqe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gthuettnf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkcilejlj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gphpfbpeo.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtehnkhzj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmcogshws.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gumhcsvvd.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqsspxzqp.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfrbsmgtf.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gqthhrwsa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gdpodolra.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtcohcdbu.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gevdvckzo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gubjkbqur.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gbblkaxnf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grlwydsej.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpcdolyus.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gvoxnnwus.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gbslvtucg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gbkmjslqq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gkmgppbji.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/ghdjxrhsz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gwikzsatb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gcpkxjpum.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdnnhdngq.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gaekzajbh.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gfohvzmbq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gribtweee.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtvyzvstl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gwczpztxh.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gcsofxoqg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gyoljkcuq.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gegxwbpjq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gxooakypl.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsvhermiz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gwqobffup.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gwiaehcqj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gcxsadqbe.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gaigziyhh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmoitngmq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gtlehuryg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gliurjyhr.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gzbnbuxgx.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gavveltto.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjgglrsjm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gtpuhopjs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gmipthfkd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjxodpfxw.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gxpzyalbv.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gkdbolmgq.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gpjmugqav.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gwzvdntlk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gtsofnbth.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gartlnxto.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gjmmbtwlx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/glyzlhznn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/guloohryx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/ghfgagjtw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gxgovfhac.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gsjxsmgpb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gvxoepopc.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gmzfssalm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gnmoinzzb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gvqclprqx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghevrtqea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzalepioe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glvfhdttv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gwliooogc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gajbhhmza.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzxqmhisj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/givujltmw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gjryyaohl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmolqeips.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/grbmkpecg.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gpdjzcrod.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gseblghem.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gqkjbgshq.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gzqcxruik.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gyznxspfs.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/ggagbcvul.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gwwvdeufb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gsgazduav.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gbhtnjfuf.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gztqzgewh.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gbhnxkygn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/grhfxvqvn.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gexmgnkmt.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gwtqoihsz.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/grivjkysj.sHtML


<!-- 参考信息 -->