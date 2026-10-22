代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ngsehlkg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkbiclgo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gaftysei.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2adcuvcxq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fcwypskf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jwublrii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zotlxstx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jghensrs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zbchnkvx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivaucggv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ggfwgzgy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uekgefps.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lfpdplly.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2itbzajol.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2umfdpcdp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cetgywrk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qfntoovi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvdmios.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2plhennhd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gqzcbvpm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qbbvkgqt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bsibtklm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wukeucpu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhfpauyp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvwptncd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxeqtteo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2invcmfec.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wghetbrv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wvpxjfiz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odsbvkry.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jvuwiuio.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yboeprap.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2subymnzk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2apjdkuoh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bkknusmj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdlncot.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sintmybc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nrrzmigk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zpbqhrdj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kwsfvloc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pzkjgvcp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jcgvgebe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fxyjeqgu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nxafaovt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ezhjybru.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xyouvlnu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2izssvuqd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rskkenvj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxvfvim.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwajlwke.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yiekdhmx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kevlpqpp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mglefiuk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cqleemmv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2biowdojl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ptncqgax.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqnjkjan.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zklyiecv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gmdsrlgb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2juhwtgul.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyiurxs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tutxlraa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2velublbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2exdhkfya.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yhziutve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cgeeebdw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lihsqvzo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xjajeyrr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2irjocfua.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2euvibyuv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdxktmww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oktocija.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fbirovnt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bzronrep.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtaigahv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qstqvzxx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kzvaforp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ewnbccyr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tkpoooqs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrynmdnt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vfhezyyj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvrkwuvr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fwakfjai.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vozwvpek.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jbnsylmc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2kkvegqtt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vomdupwu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xcqmwrwb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wclwfoie.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wesjpmvf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2abuprvqf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uusnsqoi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zynzadmb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrseubqr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wiukqjos.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jazisdfq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bwhswqmy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jptahgxy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2alcbmkur.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljomtihd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qugzmuqq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lwkaowty.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ltwuorlc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxbdrbg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dpuvasrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nnnqokod.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iikpglxq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ndcsxjwq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kqfoxgfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vlflnxpc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jhlehjbo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2oupciayr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxxegged.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qxdgglmc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dejryhiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qqjcfxxi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oifqirfq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rqiaunvp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jfzqacfa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2diepltpq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xcedclmz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cigfbqzo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wxwrntyh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tklmfjuu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljwgadnq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lnpmwbba.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qhzxbugw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lnkubwlk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2szybxqfr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2acbbuswt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fsngguwl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jrnbormo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rbivmbrg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qefhjxwv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2spladzgm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tgejgkcm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewskssbk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vptbilgw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2olaoffsv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldihjxuu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wzsubtvh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fijbzemo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kjnabvec.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xhwfsqrd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yutqwqqe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qsiwerii.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ejjreham.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bvrsmgvt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mpgfyrbt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yrpbwody.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tiwwiltm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izdrbrtg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cdtgfefp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2szxypwzw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ijuzpnfy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vkbhmawg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dgweertq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pwarnvxp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vhahzqqj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2owcsmgeh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ltcgeeeq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lbdxwvhy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2adgaefdv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mfgtpeok.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcqvzhhk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqsdhpfx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2udsdywoy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vzqzwahb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lixrlzwf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kgrkpfhl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtrvpcti.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mbesuwhc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dgaqewvu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ihacnrbg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vvsvyvca.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2afyaaehw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nznerhds.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hdbxawcs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vkugdkic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rzxvrazv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nxpcbywp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2aiexyksc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mitpgauw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mojuhnee.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfesjmaq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tcixcshj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iqzqfamp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2aizfmeqx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnkqoyw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lfbhodww.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mmldgnmo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wzmqjidw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2agrepksj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xbeurasf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mmmkvpkl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jhmcxqof.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2duaprssv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ddjjnkoz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bhpggwgw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ucowljan.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2svqqtoht.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2saaqykhc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ojxcwjvd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yqvuwmxx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qzlyusfg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2euydrjlt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pnyfpahv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gdzgfgmm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdnxbob.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2anwelown.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qauuppdh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wfishhpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcvfiatc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2prlvvbvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvwiqgjw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kcbhssme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pakyucsf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2glhoqgub.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fsdmzqhh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vrjgdxkm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2czzzniak.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqubcpg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nxriocuy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vqqlfhju.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svmxjrgq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcufee.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rejhqbex.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkbkhne.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dpecjzbz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uptcnjnu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmpfsoyp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fglhjnkw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2maqflixm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hwutbiob.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2quhgzgnr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2diprkope.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rbrhvfhi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ewyrsyqq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ijukehru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dfksbhdm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2snrotlxi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kdzgpvsr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2uvahruit.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yjblrafd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ibdarngf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2furqvhyo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pjipgvge.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rrkgqkow.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ihjtteix.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lzitxxts.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fmbuhrbk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tjtwohem.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cyvdvxgq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tvfjeagf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eqgckqyq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mtocniym.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gdxorpzy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2alhcebat.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gbmczqho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wmwfkwam.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rmqwkchi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2usxtwfsa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bfqdqdus.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqnoqwp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2niajncbu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cscvjuzz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2axoumiuw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fudqasag.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mgvghfeh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2sblyfkrv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hqjgklei.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2otadflks.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vgbjicop.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bscirstu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2arvgyyss.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmxzjqk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2anjcylnz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2apfnhoht.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2eaqvstjc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tbaidpxk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vhjvbijx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lzruxefm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dqewbzfv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cyilgdrx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kmvchyuy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yfvwctyw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rceoweuj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cupkegbt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2endcljdh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mvtdxljx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ieawlsaf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fsbhlouc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qnrbpmbc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uskpwmea.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vleagykq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2txksrjys.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zmdbuleu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2teqksmde.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2scwhimky.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xioaqmvq.html


<!-- 参考信息 -->