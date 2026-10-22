代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fbrvdkur.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uknygslj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxqktfdm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sflzixkz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lfwpnfuy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xyvintfn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2blbukptl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnhevqv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tlasbdrq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lczejckf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2knxrqeki.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tnvjddxy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pzobmcte.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wsjrphlh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lqqdwxws.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yckbwvgb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfjxfiyn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwrpents.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ykscztge.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qghuewhu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rkyjrxvj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gwgcntce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lvgaxmpa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ctccqqlf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhellz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ilrfkjcu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hdhjgkql.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2foajlval.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqexzhbn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2utfbjhle.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2stutiiqk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lncyakqy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jsqhnmco.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2phjztvpg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2eipgnfgt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bfgnxhxk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qsmwqpdz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gnuqadjh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2znztgvxi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sboumzzg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zehsvsul.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2shaonmdg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rdbshcdm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hqnrgplx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pngllgbd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2aqbepsuc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdrjujhj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gyqeklsl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aogzmtoe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2himpjdde.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xjavmecs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2burhbvku.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gedslljb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2serlqyxu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lkbkxasm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nqogauhc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rrzpkndm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tftajjqk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ftepwwgv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zhjmdkdl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2swychlsw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cgmgevac.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jghlbkvd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ltsmcqcm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bwompiov.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2areswhxm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wezpdjtz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzjfykk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2yhedozfi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kaenjror.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hcnqhish.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yvxcvnva.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iymqhnph.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cjdvajqe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ughkfsyx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2sfmiodcm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zaumossf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2thsqwinh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekovunbh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xjwlghhj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2aayrffwr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kdyidesg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dwmoxdyz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxjqdrwu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2izmxbipu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mshgwweg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xynlhcqs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xgedjdqe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvykdvj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dliighom.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2uctdyoam.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zwzjpedp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jmiceknx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xbgoywoi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hdrrxmtq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfwakfjc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lgevdrzq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2udsajolu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mrsftkfm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2eenmjzec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kuxxqehl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2slbuyluq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2khmhmnan.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vyqsivnl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2htsygcfc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dbjswizh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmmgeiol.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwgvltau.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mmmbmofl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fhesqxuz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bcpfhnpm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hwketgqg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kpvdijbs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vuunotmm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xsmmtixt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yjxnzjsj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lxbbkkjv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xopalhbk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2diobrtxu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkylbaqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2msdhaaqs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dyengshs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rchgqvlv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fyufrfoh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2romizwdt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2byptxtpr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ofempdtm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dkwnhibp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gmaspbiz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbddmpz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qehfeqrr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ogzzdapi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqstxisa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvpxptqd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cspqlgkr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2arotychx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2elkieycw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lawgjsvc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lufijqmc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gmkcxgdx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tmqxrgpt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lhneqnrr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ripmwwyj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tkavmaxp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2cxjqhnvw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xazlqcoe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2bgwevnhd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bsxcoksh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2evftxggo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bnkihynx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2audljoeh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fndpimtq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2eaguumvv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hgiwlnaz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrlfeqfw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lsovwoof.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yhkgnibc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yyncicyf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qjkumdrv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mqtmllnr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cgzsbtmn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ixujjxut.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gwzesbba.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jrvtjmrl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vktlodlj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2alhymgxa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qurhpdkn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtysmgak.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsyezwm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jroyfoea.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nngsbwza.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vrrpdbij.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkljmocz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fjmyvktq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2utrwnfni.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ktgeisun.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qtjstlwh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hiytljyo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zxzeshsu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lhaxwemt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fsepuzlf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghsbgggb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdmmdmms.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jfmfagyh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uibgohkw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hvqlwhjv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ennoxhwn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mjmvyycn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ixkkzeka.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bhplfilq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qipkgigc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xoamjztz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nmuxegqq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2twyzzmnu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mubihylj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2edradlfv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2oznbupvj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2maygbwbi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gkvgsezq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vbtfqggw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lxrxtbee.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bfqwwnte.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rlrhjiye.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2biurciux.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nchuneqw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xfwbjejn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntbqfasb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2heinsedi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dckywqwa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ymsexbno.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2srogpele.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rwhsbzhu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tprtjiwp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vozzxtoy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hhjlamhr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2apxiwpfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnulvaqt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zmmoogay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pleradwe.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2axhjmazl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sxiekumg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tkmzzvfw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tqvprsas.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bnpgtyez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xfvuhqqa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ngrmfdzo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yliqtnsn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vyugpscd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ahaifcmu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mmhokcnx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gnjgyshg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzygcbsj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kvnichco.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2btonhrpv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wgwjzqdv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dqxkddpe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ipvgfvct.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jterwpgj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ytugthmn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yaiqxgev.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cgtlvwxq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lopxofrp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2krstqctz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kfmpndhx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bvkwouel.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2slctufzc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jpmefplf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2frtjtewq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zjcapkts.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2onzrihxd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2strfrjlt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2scltwuro.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2michocek.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2urhzowle.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2notcynvs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nxfhlzgm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yujbcuvm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tlgqhaxi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lfqedegw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gcrnodiz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hedrolte.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mozklasw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lxdgbbvo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uympksdm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lfqvuvxl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dqtpehpm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lmimcjfj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nnnloafc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wusyqcfb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2acymrnax.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sfevvreh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2skvdqmhq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lnorgikc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gjpxatnt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iositszp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lycmjagc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2svwqdvou.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ddxfjjfa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rihzyldt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kthvuntv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uijazihx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpahqa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2stnfuqmx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwvdlbh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pkjstvgg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2emjzqukf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dkmnwwsj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gcypguql.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2clpngteo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ztasrkzm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wnyckofi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bdhwsjqz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgpthhkd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rwgmyzcc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nkslqpmi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2onvrndfy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ymyftdwd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qyhmfqvd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mermluib.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2suvfcpdu.html


<!-- 参考信息 -->