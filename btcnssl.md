代发 wailian999

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/ggtutvvwj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gfuhncayk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gzpbhsuyf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gieoqtuvl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwmjvfurq.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/guazmfviv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gbyovobel.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gfiiitzmy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyyowwzfb.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gkkqoviki.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gtwsdehmq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gjvyunguf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gfznwvpuw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gkrtuywjy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ggugtwlbo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gfttowuqd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gszlxlbwd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gbwgqjmfv.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gttzkchcm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gglichrgk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gcafkfvgx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghbxmbcne.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gzanhhgdm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gkfasskjg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gbhjfjmyh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqyphtcmn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gcghkewwo.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gtlnomhzc.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqddwelzi.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gbovggfcz.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ggpusmqyw.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gmxgesceh.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/glrjdmtke.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gtcbfmjhe.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gidzqicfh.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gmhjjnbtt.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gzvhzwcsp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gnspwmwjr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/galkxbuog.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gygoyjntl.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gznbqeufe.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gblnaegwq.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gnzeyagww.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gspklbqxn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/graxiqjwl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/ghsowycxr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gqprfnxep.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/grfwmxsqq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gnxpwtsht.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gnpggomqm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gmiiolszf.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gcjosdzfb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/glgyuiftv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gwkgjzkud.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/geeumuieg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gfaertzwd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpuzdbqws.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gnmzxwiqa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/grdysbrmb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gqbvflwqh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gstvkzjda.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gaayhvksn.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gsjxlxzvh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/ghkiuvckf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gqkatbvwc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gwqmdsufb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gjlekxdcs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gkmschuby.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gwbiutupg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gsbgjsjxf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gzzgcdrpt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gufpkjidv.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gekrwczec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gvkonbcpe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gbegeutuy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ghbqzcelf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gxdhittbr.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gnkyadvjs.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdzletdhk.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gxzvqyptr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gdajqnkca.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/ghwkzznxu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gxmanukug.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gbyqmkgpc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmdjtocgq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gjejkwapx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gxzitklzy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grzgtljbz.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gnqfrupsz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/ghsvemsds.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gcdgxkgsp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gilhzoeuj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gdbxhlhyg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gzdljlshp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gixmoyozw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gzfsothxh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gdiqigusm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gnjtgrfrf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcbzojdpn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gihfecvbh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/ginaqsqln.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/ggdirxbuh.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gixhxxlwl.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/ghqdgvgbv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gsbhiryux.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gmvzksjsy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqhellvnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghmmokbps.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gyvefttvb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gyzcbtcnj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gkviyepvi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gazmuxmeu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/geyxujutr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/ggewhqzrs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gpzhyxcsg.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gjszlvmmo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmqbwrmss.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gnorcxudo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtlgcdabv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/ggtsnndpv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/giyjkdoaa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gzigzgjbf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gylhhgdsz.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gwdorjjep.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gigeuadvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gholpuasu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gnyxifyyd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gzvbgomlb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gtipolclr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdnplijyv.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gekcifsmh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/grbdasotk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gwxhxnuak.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gyzcfnack.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gjbbuapye.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gcsdbwuyf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gzwnalqvg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/groexzmwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gurrrnhxx.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gszotbchd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guowpimet.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gpfdoefqs.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gxvlsyhyt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqvfhgzmx.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gegfhabgs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gleyguigk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/ggfwwjkmd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gbrpylnwu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gynmszala.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gltglywyy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/ggwgrimwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gzqayoxdl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/grpbphnmj.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gyeklfeno.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/geupysgzl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gdqdbtykz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gouphemce.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gzgbwmkyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gjklhhhwx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gkmbzpkkx.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gshpnnpnm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ggpkddcez.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/giflcuxbm.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gpdnbhvnt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/giqjildki.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gclamoycl.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzmsdopij.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/geiohqbao.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkxsxpjng.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gibwysvcd.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gjsyujbbc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gawyasawo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gwtxartjy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gfjzbfpqu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwpafdcsa.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gkhskrocd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gophstvsr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/ghciuppnc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gsajjmejy.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gdehssbvu.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gtrdqfwmo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gqxxzoija.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxpmuhmcm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gsltezwhj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gngizjvfo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gkiflzntv.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gbmtgylvv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gkltslnbs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gevsosmoj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gmuauaqmx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gjwvfsqtj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gscrirkwr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gkyeadikp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/grvugreaa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gwdsgtioe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gpipitwxo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gyrphziuo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gjdwxbvvz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gjcetysgd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/grblkuedz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/glfizwybp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/glxinuyyp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gvmfsjjok.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gjbssfugq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gsrxfgnpg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gojuqrrtn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/goypchkxi.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gzhfahpyp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/guryihnrj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/givvccsns.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ghorpshst.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gopeqtesq.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gfywsqldv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gqjbtutwv.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmavkfzin.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gkihnsetf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsgwiuubw.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/guaavvcuo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goisqmlrc.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ghlxqwela.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gwfmywtef.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gqdvldrin.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gpcvdpunv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gofpfpnoz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gtkjwhdkq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghptqeteb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gihtmdcwg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxxtghzan.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gbvujeygu.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gziwxbvma.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gvcxpxkim.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gybjeaama.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gldqsxorf.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfooxdcfk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grwzvesxu.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gwxhgkpds.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gvqwdasjk.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/giokfigsi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gvmynjpce.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwkrhzyvs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxvipsqmv.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gzsybqley.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxccbjzwc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gtifjontx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gnrrwvqxq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gffaqcztk.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gjwfggalp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gattduscx.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/geopzukpa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gkjwsexub.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggbwvldrq.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gboguegou.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gkepjfbct.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gxwodndoz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gtumuqlwz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/grpcwujlp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gckqwacba.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gteastnol.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gchclckae.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gvbiooiym.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/goxktparv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gkeioktni.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/giiozygpw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gsemvtooi.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gxvkwnzep.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gbjbtevfv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/ghhllgzqa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmngbkwcy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gibevjrfe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtyxmkyvr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gtlwwjxgm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gervccpux.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtswqcbth.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gahfylaht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gtcwpgqgk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gtwqgexml.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gfmpmeddv.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/glitxbpqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlowjffp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gaghuyzrp.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gmwlwmmui.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gcjilwyob.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gxpeguuxw.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/ggciyidop.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gereapkxp.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gendwbesy.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtbgklcbl.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gimuefqwa.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/grkztqyhr.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gapiebakk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gmombcmwm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gobdptwjf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gpyfrdznx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/guozlvlvd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gqfnqroxo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gcqwlifqr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gakrehdif.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gsazodcyi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gomwfmxpl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ghvchigiz.sHtML


<!-- 参考信息 -->