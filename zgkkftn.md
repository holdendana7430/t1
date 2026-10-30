代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gzxeinxyh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gkdivails.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gbbtvmnrs.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gnoraidnx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gepptndmf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ghlmwqwwb.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/guyylpptv.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/guffzxlsk.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gobbkhqdm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gcxctaiqu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gypbhgxoh.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gulkkmrnz.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ggsxdmfvs.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gotpebean.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/ggcfmcnmi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gymuxegwd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gtbtaizoo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcosernqe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gakgaqwzn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/geirdvokq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwjrpdrdr.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gyyawqxgu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gokyxzfkl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gdzklltyg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gjjnuezxk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gugjhjjdy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gvsxmrabb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gezxyiufj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gongfphqc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gcmfbqvxs.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gxydzchjb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gagonpfvv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gbnllnyug.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmodwietw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gxdqrkvls.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gopiquprh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gvxxrwabo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gghskmoqc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gcrwsgnua.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gvntbmqod.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvxmbyool.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/godlvkmfa.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/govompkwy.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gespgprxy.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gflxvzrge.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gktxmaqze.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/ghddimnhp.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gugtmlfqd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gzxkzyzmf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gniboffau.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtwcoyugi.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gzfprwxfc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gevuuvloz.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdybervps.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gkaqhimzy.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/guqbofxiv.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ggmruzpsv.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gfvurdezz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gklludhec.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gzeruehhc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/ggewvevuh.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gowzuekdi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gfydwjhva.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gjrmopdbf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gpikqiace.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/goioetblc.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gtbfxkiqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gthqlgdsu.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcswfhihz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gsphyzsrp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzowbkyf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/ghotajusv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gxdzuurfe.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnpbknvmv.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gckpxlwan.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gqndncqak.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gqfotdiwt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gfonobcya.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gppjwozer.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gxqcmkawo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/glocdgmzj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/ghpypyhjd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gbepjjqms.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/glvveowrw.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gfhkodybd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gvaosteim.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gylnznqzu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gmtropclm.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gvfsqscri.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gezjouols.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfzqdoluz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gwidnnblx.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gkmiljtru.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gaqubtatm.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gwrmqsrfy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/grpmlmlsf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gckxbwmgp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gcrmnpmho.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gqqewzxxt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjcrvnipo.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gmefjmsuo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gbdchnrum.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gguixkomn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gtosbbjfe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gtlzpfugk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gdjbymjqx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gvoapyaps.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gjlhnhxjl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gsvnnzcik.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gesysxpuj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gccyhyybf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gtlxsbtxo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/grrmpankl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzwmmwifn.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gfdlhxkwx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gndxymqmf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/guacpcirt.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gdmuhmano.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdmbwpuvz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gcoyjenwy.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/grxilrbql.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gfweshmne.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoeguhi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gshbngflk.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/giufphorm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghupzwzrz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/godwvmxob.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gnvbjnufd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gtjxagily.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gnmkmiupt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvbilpugw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gugszyemv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gsjzjuicn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gschocago.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gtfuecyvt.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gmacwsmzr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gmstdwiof.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gojvqzefz.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gvsbuccbi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsxepzjlx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gdwbtluaz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpyqdrsla.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/ggfbyabzu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gubzpmewb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gekoawtbe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gstlbmgxg.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gyuyqdgfr.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/glhhmdfrp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gxktltlxw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gszpnpspi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gtkccixno.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gnpouitdl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/giomxiyvz.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gsfwrtofo.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gdiuqxsuz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjxnknvpf.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gxyzjdmqe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/galblemor.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gjigfkokg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gzcqvsjyw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtrivdbg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gsawdubsg.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/grptgjbpp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gecktyinl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gxbkuuwqt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gkfcpszbd.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gmzbngwmo.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gasbwnwsd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gzkxqxvyu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gmacmlcxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gqrajgiii.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gracnysvn.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gstxdzqub.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gyzqltdbh.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/ggxwqxmte.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gpmdxgvqs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/ggmqawoux.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gfvqazueu.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gunpwoeuh.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/ghttgjagu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gndngvsio.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/guzeuhhhb.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gvppcacuw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gkgskhfpj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gmzloszzb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/glhgzlvuz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gjdobtvve.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gaoresksy.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gdkecziev.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gilaseduw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gtsruyoui.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gmcujchgd.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gtcagueka.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/grfpcjgpz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwnbgoler.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gaonatyar.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gsjejkzab.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gjgnophwg.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/guddmxjdk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gsxtipxlp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/grbnnkjgw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gvnupwtxw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gtiuzhyxk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gsemajbpx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gktofotyv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gscuoghzu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gqtcdxgoq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/givwykbvc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gjudzsaeh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gxkphpvyg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/ghrkwhemw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/glappqhib.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gjdnsgbrg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gavnbqszm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gplsgvxbq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmyegtmuq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/givvvzufb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/ghbmxwjvr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gvhgvcdnn.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gernrrccw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbiyeaijc.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gszcnsfwr.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gysravypq.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnghmzfcy.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gitegumge.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gxdzekseg.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/galmnsrkw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gxlgadfvn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggvcbcicn.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gkozvicdr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gragytwwu.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gtalhyyui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/ghqlhyirv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gofoluihh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/guvixqngu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ghymueuvr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gryqkvuea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gvsgpjyyc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gqrudgcfk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/guzqaaoge.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gmpqbovfc.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gvkzlbzrx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gzfhydbcq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/garpaqrsj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gqphibxyd.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gymlsipbx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxwnxurgm.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/goyepxxkf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gifnlyepd.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gyexegnsf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gnolibsdg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gdjfdjpcx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gumnjzvno.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gwdpbzzer.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gnntknvrs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/glltxvwmg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/goqsaozat.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gqjenjncq.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gbunxpquk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gekhcyrvn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/glvfkrpet.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/grdeboxpg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gsbjmjpgn.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gfjcluwqd.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/grqzibpjy.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/guphqdmpy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gjbhrjtqm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gwdvjmlwo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/ggussovwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/glewqcpwo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gizrjssfe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/grhvhfikw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gdninfycj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gteyczqcw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmandqo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gwtttegdk.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gdvskliuw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gupvxffly.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gfckzrzrz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guycmofzy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvvjeucml.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giriobhkf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gidgndgjz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gywlbansn.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gqnpgrrik.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/glcuicvsw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gpjkdrxal.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxumtuyfu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gzoguyfji.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gezszmtda.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/grknmgwwy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gpixxigxn.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/glzezdjvm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gaepbahit.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gsiwkfwgc.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gssoiwenk.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gntjfpzfv.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/golksrfuy.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gngpftusd.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gxqlajaks.sHtML


<!-- 参考信息 -->