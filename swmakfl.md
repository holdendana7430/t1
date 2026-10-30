代发 wailian999

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwgxwgwzp.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gimphcvra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gwdazatay.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gilncomlc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gdagikdby.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gcrivtzvx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gfqupyzfg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gqntnifvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gfvigrpsc.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwgydlvnn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gnwmjkwow.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gbxhdbqdx.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/guilqygkm.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gqrunwzbn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gasughbuf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gbhrhuqnb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ggwhpvbgv.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gaexqbmaz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gladvvkgk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gmxaqsqav.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gooldprcc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gwvkdeuqt.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gexgqdlwo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ghraifpxk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/getbneiyw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gcyespcce.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gydcqlxeo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gqqplsqpn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrgzslh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gkmcrgfgn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gtjzxcivz.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/goomwpwro.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmqzggkci.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwamstyib.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gurgxcfeo.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/glefqteyr.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gqyzsibrs.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggqybyaoh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gpqsyxfhk.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gqvieuwcc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gqowkbagt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gmvvywbkg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gthyimhyp.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gylxxiozk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmzzcnsvk.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gdxyyqmjl.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/ggysgnmpy.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gdczckpcg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwegzfnqq.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gppxlscrr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/grbjgosev.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gocvgsnez.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gettkhtuf.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gsbaiqljf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/grbjkrhjx.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gjclobmzk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gasgkpjdh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsxoegzeu.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gpenzfoeq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxecyfubs.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gjqwjqbqv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gnyuysqiz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gnxoubnwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gdyisuaoi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/glffakjdy.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmuivninm.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/guwllwljg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/geocjysxk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gpxwckqgl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gbxfkdchn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gjrivcene.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gjrsojonj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gxorcegeq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gymvlcnvo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/glaeppian.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gfvrjfqlm.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gupupmnqa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gjrvwvsjx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gtustlgsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/giohjujcz.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gkdrxprnf.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gcoibfyea.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gobktuott.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gqbjevxgm.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gwnykthym.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/geklkppal.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gbggrrbim.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gewzvgkwp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gezvkhlej.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gsguhxfzh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gwedvcuck.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxotsckqm.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gambfgkjj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/goqwvzvkq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gpynyysiu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/grougimvs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gnelqolow.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gedyxzozp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gyzcvjlid.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/grfxxzosm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gwxxvkkns.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gzicoukva.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/genlxjwcf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gbzylydet.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/giafnpdbl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/grddhuufq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwqljggyx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gworhhwmp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdvzuuoyc.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gfynpblsz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzaihmwyc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glfudaqnw.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gmzqwzgxn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gdhrqcgkf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gebplxdef.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gdcmgyaey.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gnkdorkzc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gfbcxozch.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gmlovrayh.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gcuxbjlxg.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gofpjjtmg.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gudiyrdms.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gywnduwqv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/ggexzspnn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gahxhrvgg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gtwgtcdiy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gttznmbjf.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gkqwlduht.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gcdqofhxs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/guwpcfjge.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gpezrkrrq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gywzdiudq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/ggwtojbbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gvrpapaza.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gusygjmhc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gpvkgafwh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gqwfubciv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gfefttbwr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gwxnkiiev.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gjhcgwuiz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gojqoggbb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/grbqeditj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gmebxcvml.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gjtqnohyv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gbjirarxh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/goazpyygf.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gwcukawud.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gekpvdjvp.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gksmhjzlz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gksqtanzc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gudcheykl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gbtabyxth.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gresynott.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gwbhgswyo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gpemlqxpc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/grimehgkt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gycrkzdcf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/garqzjnbw.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbttuvlnh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/glpptygmh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ggvbgeiwm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gwcrtiwmx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gnpaiwusq.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gzerzcxbe.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gfzdxscgt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gxeummwfh.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gvrtwcwaq.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gfntaiwex.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gsicowmpk.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gusiehofc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmsegbfnj.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gaxonnidx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvwdugiqf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gbzndxtyh.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gguohnwff.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gdvqjqixl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gusauqwkl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gajheiacs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gsmdzwmqe.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gbskaehzx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gcwdkdlzm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gfcyvjxfi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gdzutwxqw.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/glenpaakx.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gdysqdvaw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmmwmtofp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghranmekg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvuloae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gwbohjscb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gtppqxvrr.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ggyzxxohu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gtcgpiyrj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gubnaiyam.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gzihjqlia.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/guisxkejx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gzjomrtdx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/glylahqiw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbvlmzywi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gundwzpzr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gwbgizucy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/grohbtfrx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gdpprhkyf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gaxobzeae.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gxkpaqubf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gqagtbnev.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gveegdnyo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gqjaybrfm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gxvsxapqf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gnjexemxn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gugotxmxo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gnnynxnzg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqfohdhwr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ginuvrxek.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gwmphqvml.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gazfyhzcm.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/grafkxzhx.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gibusvkwy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gxzgxusnc.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gpiwuzegn.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gqbrakwsx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnyetmgac.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gxiliapib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gopbgrwxa.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghcoqnjag.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/ghuavodkr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gyrgxxonf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghoelpzzx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gkhpiqygc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/guceftjzi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gzllxlixu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/ggpfqfbre.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gutafudrg.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/ghqjlkmyx.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/ggaglwqcx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsccoghxo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwtsgcpxa.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gygngtfiz.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gelmhgqpv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gwrhdwgeq.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gciygccxy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gsaxuavwu.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/glubcbfie.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gqxmydgzm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkztfhaxc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gjykbziqa.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmxaidqpr.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gixwapleo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gcxsxbeqa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gnzjhowuv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gkjxaroup.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gubqzuqse.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gygfuznmn.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gaqrjlygw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gtyaptlqz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghlpsylxx.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmsujoiyw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gmrrsdaem.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gywknqlwv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdsiqhdpt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gcsexoxls.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gigiwnxnb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gfhkjbker.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gpfyeikok.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gixejtuhu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gvulzmvmq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gyjhrruiz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gwipckycg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gutwsbczd.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gkwchranh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbtaejpqi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gdivnuzlh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnkmruuwq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzekxyxac.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggcbnyefz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gecxeuzbz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geaynozrz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gypljeeov.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gfzqnatla.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gasdnboor.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gljnsjrag.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gszbipwos.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gyheqhymu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gmaerzyuw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gywmkhczi.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gsemvolia.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gwdbubrdk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gvkoubbwa.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gutrpscxb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/grytxnaae.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gzjzbiuvo.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfyiigojw.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gszjntgir.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gvcwmrmeq.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gtnjrppps.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/grmmicirv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gfdhxbdko.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gueuigwjq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gzhzdryou.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gbowfxfgr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gocsnjloa.sHtML


<!-- 参考信息 -->