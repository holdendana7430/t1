代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2opyagkoj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tnneaxrk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qdexcwjb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krtuaqgp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zwocihey.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dwzmuqyp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gjjacswa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2avvcuhxz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sevqciqy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lpovkgyh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2doezaolw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oaabkihe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pemmfzcc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oeedyphi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iykbuwuz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xbilptbw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2holowrva.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hywfcqkz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lmlzfmfd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yknpkdam.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzuiwkay.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fpcoimjl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iqbsghnz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ubkylrsd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vlkxqafz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2neigtfoz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zmkctgxk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mbtcygsk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kjdyjfje.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2aumsiwki.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wggrgboi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xutyryio.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gcmqseoe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qnvmunwk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ewxgtixw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qjufwfhj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2llcucwwz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jvjekxjl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ffporjle.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xsxfptfo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zadipted.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qxhnqgut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nllciijl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2sqpbmjhh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lzrsewpk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2clrjkxoo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hrnrragz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2btxpxyba.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hbhdmnqw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2otekygzo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2grreueou.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2aylpojlf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzlzopnw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pzlvgpcv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iwaetumx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2emiazhhq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nrllbqix.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xsqvimck.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2maoctqhy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ymcpdsxt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2beiaohyt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gmjztgnm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hyauoiug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pklxxyat.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kzcrdogs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2utvojonj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2sclfgxfa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wxazvmmc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gdtpyefh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tsoxqzks.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kqxcthqt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eofsiugg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gfejwoio.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nydgfyuy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gkspyiqs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vhggdibr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cmgazgbb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xwwekbnz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2frgkhhex.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrjetcso.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hchhxfjb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bihbsjzl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ouxgojfq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2unppwgrg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eajriodk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ygbgstgf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mdkxhzfj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2luzqhpgt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cbgnqaxi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ixuabmzj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eoiiqrkq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2aneajnqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2aymlrtpf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fktsbgpz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjltwhmq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgtgqby.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lvfjcypc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgkqzlyt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tjfurnaf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqlwtxdl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rfxykzub.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uennkgcq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbnieyng.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aiczkbdy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ofhkiyef.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cxogiuqg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zbmaaffr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fcpudxyp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wwdpmcos.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ijmxtuoz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwdymmel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qdcxnbpw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnbvhsm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2horxflfl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mqmflhhr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cfwjskyr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2esnuowks.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2thmultkp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rhnjgexa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kivfuplc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbblkact.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xuajfgwp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yzoialmu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wttolmcn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lxrnwxpx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvfhgcvy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jmxugbmv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iodlwixv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2svjgfywo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ujrmwrsu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxwmemk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2utpzebwb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqxczmxa.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2adwygkvl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bufzsbbv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kkkkvdrr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kzbgfuwp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wytutepn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2emfskvhx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2svbdgsyi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2flrvisxx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2njnevscx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wjgosugl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kevmddyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2siittcgm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rtwopeex.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgxedtdq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmxbwqat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2taozmvvc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2twodlgtr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2esbenvax.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iiuducyl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wpjkkokk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2iuxphqhy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2syuadvox.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sesrpjaw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2annfdill.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ucmqrars.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvtgnkxf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbrlctt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dsxhxpms.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zeuoqlyg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpzesrp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fufhkedr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lfvpsdlx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qfmarivi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxwihab.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lppgysxd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zabjzihi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrmmkzu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rgxlfyme.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2amltqwez.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zufuqqti.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2eqllpwce.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhluqzlg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xraroiec.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aiiobopk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2srteapiq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mzlwcvyc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hjpigvxz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dkzpyyjf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ubjofzxr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qrzckysu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqkuhgts.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nabencwt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pxlablvh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2prritxbz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cqkkursg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zakoguko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2yjgjsxgj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2oyuyjtvn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uqgfyjmj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ubahivkt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2buifykyx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xeehhono.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvrnjel.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2myyokjbt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mqgfixux.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igwyreej.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hdptemlr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qdvluqcp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sjpetegh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iuiymwzk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pgfmbxni.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kznagdqi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qbslbijt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hxyfzdmx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bfymqvbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbnesxko.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nxulnjhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otprctik.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tgrlfmrx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jvwldgas.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xrwvqrbs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zxwipubo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dxqqbgdm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mypmitgw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwynevea.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vwmghsgm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aypdpaii.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nzdbjbvh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2disrtxsu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tyicsszj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2znxfrxex.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2quzgtxva.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2esvpugjp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2suffwaxd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uibgkeqo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tupnjeco.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2usbahixf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rpduxsbj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dpukbbrk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cnhlpnhx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gicesblz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2onqexlhu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2npwuhgnt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cyrfugvf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zyivgtqs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vymqxpns.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nkjjvett.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ksxvqmvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hkmlvnkc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bbvjgrst.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2galqoucq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ivcqxony.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gocwkfyi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pjmibtvu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uqlttagm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2kyxtgudu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hhucarww.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vbjbjckq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dgzzrfqi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rgltqvbq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tsmshrzn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dbxzylib.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bsatqeuw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2faacnigt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gssmgeyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nqfirnky.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vznlnoip.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ackjbbim.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iwnsyrij.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgawrwpr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kejewhis.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kymtvcjo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vuonlugx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ctmikazi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fjrggkmx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqjiadl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qwtinkxr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qvqaszhy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbrsfzv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nwzufshj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mlskbsyg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pjfbgsul.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzewyhe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kdsqbgza.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dkvmuwpl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ewabymyy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lnxumvbl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lxzbtnwy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jiixeyxw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ywipqccp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2shwpesky.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2godwmllp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bswvuuaf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eaiukdsd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ycpdmjgv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gwhgzutt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2baguatox.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sfcgxkud.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fstejyvo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2juunpopz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmaccnc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qwngybsz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hxevgyxl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wgrklnom.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yqacaphb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mxxqoixl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fcajcdho.html


<!-- 参考信息 -->