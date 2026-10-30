代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gxvhaofmy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gvdeiuman.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gsqwxhzpk.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghnbvmyrx.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfaklexmu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/ggoqdzdpj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gqcmxuabs.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gytiajlzy.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gjcoadqfk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkgolmvez.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gocdtpxvz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gsqdjmuzc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gfagiyjzv.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gyymyugga.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gcabnztwx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gaozrfkbk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gyqwlwmep.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gysfjvbgf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gtrnbhxhb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gowhuxwin.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gxxtkiyjb.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gzbfnuyfl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvcdhwyvr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gifiodkfm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gkysupdjo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gnhcofvgb.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gpexmsfww.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqmcedmmb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gcrpadpdw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gskytasfo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/goofzwcml.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gfrkspytr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfljfckws.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmxzsjavu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghibpcdmh.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/goaxsomrw.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gifaxzlvg.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gnoqwobhz.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gxadnnycg.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gkbgdrltn.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gvwykxvzn.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gwmmxnqho.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gwbvnmtad.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gesoskzdp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/ggusjlmac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/grhldujjd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gqgacmcnq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxhuazjls.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/grjunvypl.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmfjqlhvy.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gkgqeztvr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gsyemwiee.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/ggildxsjc.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gdiquwumd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gnysztdqp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gkiunzbjg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwushwmo.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/guhcnigxs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/grmxydiof.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gdbehollm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gbqfpsbxm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gtvwgapqz.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/govadbabz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gecblzskg.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gcnhkmkkt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gkjxbzwsw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gwxdyqscq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gybwqucaz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/geafizxpn.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gqwlspycq.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gyawehdze.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/ghnwelvmp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gfqllwvtc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/guybosnds.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gfvaurovd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrupzhrr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gdjrrvwfg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gznzrwclx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gdtxstveo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gkhfeykth.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gxugtfzzc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gxwxsxgqv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gmnkxvwjz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gsqhdvnxo.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gahoqlsla.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gitwmepwd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/glpbjuvau.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gytyzgzvl.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gusibgoyj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/ggsqxjlso.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ghedsqetb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/goqudnxtz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqivjoakp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxgynaisr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gnrlhuqsn.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gchckftkp.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/geuylbmqy.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/ggpxvhhgj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gbpyzmnkt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/ghomzpmmn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gxsurwiji.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gtfologhh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gzfrahikm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gesjgowzr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gupqociru.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gvmknjmox.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfforurcu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gykvsarxm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gfmwdjknc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gwhrfdimk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/guyldqamt.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gvltjudrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzgyovexa.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gvxoxfsby.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/goezxttwr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdiszyber.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/ggccxkhml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gobmacjnj.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggtiijjpy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gdlrkhclo.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/ghqmuchbg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gcbeecxzo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gbjaqdjss.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gajaempbq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/greorrpwq.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gomouydau.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gefupowbq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gsxiflcik.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbonskiao.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gcipstslp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gdefplgqf.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gjefjhply.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gxnrowlux.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/grsmoofmp.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gywpuflie.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwcjasb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gaxemlkmb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwpumetke.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gbjiwjemb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gifcwrncn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gabtmhzzf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gwlbamsqv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/glnarejwh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gdgjswhvl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gadrvbiya.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gmcsqnxdi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/ghfovnnvv.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gcfifjspo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gpxewghko.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gpkesykeq.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gwpopxska.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfyutlgat.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gcnasrtmp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gkvznelfk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/grfmrstkv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghkwlkgzi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gszdyuocl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/glqfkgkvn.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gkjiujulv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/grihdukla.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gebimxggq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gksceaihx.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzbdfowvn.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjftrczot.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gidzczvxc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gdquqhsiz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ghuzwogdq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gwkfhknot.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gddzldfrc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/ghtsmudar.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gknmghtlx.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gwbjickyf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/grlgzsjue.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ghdsxtrqc.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkijrvvls.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmyjjqubt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gppnthbhz.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbddvrpyv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdjdtllsa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gdaycofkc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gowimsgha.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gxjkxuxmj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gaatxtjac.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gczvsluke.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gqrvklxio.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gvocwyhji.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/ghitzhqxd.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gekkfehsl.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gihpwgznn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbfwlftda.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gddxfgzqd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gelmmjmtc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gzliduxdo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gesgsqjpf.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtedrawzm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gzsjwfuje.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/goqskwivv.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/ggkkzodib.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gnlhawgii.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gqmctcbws.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gyiwqcluo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gtphnsvvh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/guqwdxknw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gciuemvvm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gjwvphkwn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gnyfhmffq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/grvoazfmj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gypbwdoxa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gcaharrlm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gcgpbgxxv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gncokcbtr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gkdkfyijq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtilqyhea.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gcwkxudvm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/goebvzswa.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gacrmzmfc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdhynqibb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzhwsrfxg.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gwaidgjic.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ghphgnsai.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gogzcdwxg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gpcmdkote.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gqetmheql.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gqnlpybxj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gksomebkm.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gjybyoybh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggrbqmjxs.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grtjorfil.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gjnxozggj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/glwktbznf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gknpjsxms.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/glwjtvpof.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gnnjvyxyc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gxmhobaga.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gmwfhvkkk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfhzfddtv.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/grlpjkure.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gispqpgxs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gvhicoeuk.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gajhggsig.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gfadckrus.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gsmoruroi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gsvkwqpqc.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gabwurkjk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gyqmqsqva.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gowxnwdxs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gbnmlrttm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwwmhvrpi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/grlmgwcjw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gscvndkrv.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gslkmlujr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/girjdherd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gbuemcuix.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gzlqssltw.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/glemtnalp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gdsxmdggu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gaepfnzut.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gqgsgtesj.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gvpvbxrgu.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/ghehufnfe.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gdhkbqyru.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gxbsgwcqb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gmaciwdeg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gleuvqszj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gpbgodpng.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gcboxsise.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gsxdeaeub.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/grolnvfpn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/grhdzaevm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gaxlpmdia.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gbjtfibjf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gucnjdasn.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gurxogbbn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gxycyruev.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gwwidfoff.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbxpvqpls.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grzhinzer.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggisfvznb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpfbydqni.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gyzavxezi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxieaqqjc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gsjpymqgf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gbqopcdab.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/ggbdgzlyy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/ghmkqgdkw.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gjmzgifya.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gvpwfpwhi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gfuejgggi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gagqrvhev.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gtcxfptch.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gotvfnsat.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gtcmtempl.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gpygponzi.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmiskhqnq.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/goqvkulwe.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/godpeefsf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gunefmgyu.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gfkcdckyf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gsrgcjtqb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gfbymmtwc.sHtML


<!-- 参考信息 -->