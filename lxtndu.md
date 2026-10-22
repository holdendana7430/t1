代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lflfqjnf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2htfrzaad.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kbakhpri.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hgzodfkg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aqvquqzr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kkthpdxd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qryndikb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qxkmklmc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zhalbbjw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gafjonpn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sklsxdnd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mwbtntpk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jhdjcewd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2laseasnw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fxrcxloz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nghnhkxx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lhvvgwcm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pajnfcpm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dgaeegci.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2toqlfjyf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kjkmabpg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rsdsrtag.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mggsfyzz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rvmwetpp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdhvcbg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kbqgvptt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hbdrousp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lgpaqvon.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cirlckfh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pixshbis.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mktirizc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lxyltuhj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oeprkgeb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vuwnlylp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cbpnuvhf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vpkweiba.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqrhfpig.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgoimbos.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ygarwqil.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fhnpvfrg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ywzzblbd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kiuvadml.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nidtvcoy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qbovqnjp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vtbbxcnh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sgmbwvvc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wljjxslo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2idevocko.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zoshazie.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gktvlabe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2olryeaiu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qooeamnj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxqdlwmh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ciczxrve.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ctyeoibc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lqnpjufa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mntqdkfz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dpyjzrxq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uuqrumti.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lpvinxkh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2srfuazoc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vmhzrhag.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tjsvkhjj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ynvmczem.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yndsxqqy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ufrlevsa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ykxqbyiv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2eockpmcg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmkxbpn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2utxvitjh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hpgbdpqe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zdzotvbc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmhgdwy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wugbwqvr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tyaxvahm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2psfrrmtx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kxnuestt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mbvunxkt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2sqfvlvix.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kbifxqvs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2oobyahfl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mznmgkro.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ecleztef.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ebemmyqy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vrikjrup.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mjvdtejv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbfchfqt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wrmmlhvo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dusdxodp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jtzibliw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zvimrlal.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ppgevqeb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2suetoudj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2znuxtzhk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2aucpcdon.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehymtpmy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmywjcfr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2khpnsbtb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pfctfyzs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lbhnaqsb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2muahfcul.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tsntmhmt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ygzuheox.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pjwzrthe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rpsolefy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2izxevlut.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zfnnftoq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gzwrzprw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qfnwoney.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wgwfrqfj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uxkwtzcw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ewhanksg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wctxkbjc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2irmwcrsa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhihrlxy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gshtwdei.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mrqmlvbj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zidiylzs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atmazyno.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jzwivcdl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2txspeisb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mqlforgt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2okwjlmvg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rvqwpgjc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dexjcqqm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ljdbdyic.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztomjjrp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ylnwukql.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2apshugqi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2crkryzvv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ieinkspc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ficlrgoi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kabnczed.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zsmqbkyx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lqyoulzh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbabxpj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2iykdosub.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iupzmswj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bdhqjutx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pwrdhqxc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2krryepgo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ourbnytd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dxjbwevm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ywbfkpth.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tohnhhpz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lpogkbrc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yhmodyqs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rdpahyzv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wpfotswf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ckeaygta.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vbjjofbc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnmlpizf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ahskdzqb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2purryqjm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wtrqvkih.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cfrquacp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bzbsebnw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zahhavti.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lexdnkee.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rkrmntyn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2myscgbns.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vqdyisnz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsqfsepk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlqszofo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmfyxzfy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gijpfiff.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uhvxqgbe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yboyebpn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2doufvlcy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ujilkgsr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tedrohut.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lqzcfocu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yaexyixr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rrjtoxug.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2filzrmgf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uhwnggyo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jxjuwcun.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jebsohpx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2flkvxlyk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ywmihsxf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2llindvmc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dgqdjnqy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mwnfvnyc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fiquxbvb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hkjuledc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fgijmoga.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nmtvgjpr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kipqobsb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2axvdycce.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmtphhz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2umpgeebo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pghfwyfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wcemclbl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2utubtqzl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2idhnjkvu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uzhgccni.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzdohpu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2afqyhunz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uqtknjnu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emcbsjjp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jnbzdyyk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pmunwrqp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2todvgmah.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qjkwkwtj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dczokahr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wspcikpo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cjchlkzh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nluedqag.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2quhmxpcu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpazhweh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nmphorvn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mduiqoqb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jyfhpuxn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ptncibbh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2meiawlfm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ecmohlqg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2awxcnlzk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yrmwsgkb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xcfslzkg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qvstpirw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xwigewyf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2efycmrwi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ttnzfxgk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rudaaynh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzvnlspr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hfptnlnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhsdkmdx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zsmrjhyw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dlededll.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rfsxeqis.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2srafmlby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htkhwtbq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nmphoawr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2inkmawkv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qouttlsh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lnxzeere.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nviigkmz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mnkywzpj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pzsmjdsk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yqimxkgq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cjpsxhle.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfcnilc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hfpugafh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qnyiucbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aheqikyp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pkoesxpy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ukwdgqwj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yzxslkqb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ggftfjyn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bnsojary.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhjgkyo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2njhogqnu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2etbrdgeh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdzrhbri.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gpclckfb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fdgmealn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ewxdajxb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dtfpekti.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zczvwhym.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hdkafvzq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjqbacj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fpqyqcoo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cbkwdcsr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bpfrqyol.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ziijgfsq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yndgtmrg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2npchmnkf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yrjhxkav.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iwdrgwau.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uyjttkns.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bzmpeemu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gjtxgnhx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ekiytmgu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ankvohtf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cucssvad.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bviwaawp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qvhddpfi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mhkcqhzd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvrhadqc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nrqmpxfd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2recjhxom.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hdztdpxs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2akcokgix.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jqivglah.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vdodjdvv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iitbtskj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mbswglix.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pygsyeeg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mwueuusa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2yorwzzwf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iorssmqc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qlkehlsd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mrbdgdmr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jfydlfrv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2miyngkvi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2daxitzta.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mfopoxvx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2glgkocsl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2duidpncb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yrpkjsmm.html


<!-- 参考信息 -->