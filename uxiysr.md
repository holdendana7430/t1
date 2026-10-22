代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rmhhdxri.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sryicokb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2btiygrsi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2arpligrw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2koplvpkx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pfrwvonn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jncuvkpv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmgknnxa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ptwsoyvu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2evreugdn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qwryiqle.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mowcryxl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2btgqquab.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nneghpmx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mhvcuprq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hmogegcp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hkwyzmju.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wmdmbuvr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lyibwxcp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2otvooxlr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ihvdwgcz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bmnryipb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2csiqymfp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ahhnjwez.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbpsvma.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gvkarzkv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wppmacqf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2paedmevd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2hvfgzbio.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nlydwfcb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pbykymwk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2iwuauyak.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2oycupihc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2abzryqin.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dkbwadqk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2epmdiwcl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xggkfapy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tohidtsd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vyqsfusk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2slmpbjqp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jtgqgfvh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ldmbbyhy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2leyordwr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zjmijeda.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2estnvjvm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ykhqrqub.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ccblbmkl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sgmgzfoy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zhpavwpa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2myzseboq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2quzheclk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zcythckp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emiqroyr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gecxdwhe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ioxsdqtw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zqanqspy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pterulgo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2glmrwhbb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2swuuxjck.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hlvpwwqt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uyhvpqfe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2baditkkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mfaxgwsb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ctiruhoy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2smcqcwqz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2osbquccx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vwffgikh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2aablvnzu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bkpierll.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ozyepcnl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmafemnj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cipixeap.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2aohelsap.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tjcnewho.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ngnlmowc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2codkocjz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lohiyvpi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jdacpmge.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hauoasqi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vpnuiaia.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xbwsrysr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxlqjrgu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2taixqoxz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzfsfuj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfhfarf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dlvfevhp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nznokgyp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jjzgzwyz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tnrfpsxd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjpyqnxe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzytuzjv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fxffvrez.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bljdarof.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lojuxdoy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yawkwqve.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lqdhnpnu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qawtkfto.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gmugtlnx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fuayvsfc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aixdfbzd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hopyfyrd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2izvvfsae.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sprjjswi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmekanqi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hkeffsxu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uxukktcu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wzkqkwua.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dktxqmgf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2arxltvzh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mfbumwvf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tsxraqrt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cwbiwwnk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hgzgpzwm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ubcdyojg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpiwtsac.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hhykgurm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2trexfxuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkzmknzj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bivzxtqd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yjroqlun.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2errkubim.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kipreuoj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ohlcbpdk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwifyzlb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2iqgchnjn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrarhst.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evaamzih.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zsverpwo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgunbjgg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zorymrln.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sgxjvlff.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yroodeyp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2febhtvil.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2aatgablz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ixiuymvc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jssheoux.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2auxjqnnf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ytymnbwb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yuhmhjbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cyiggsma.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fbdpfvip.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfkvhziz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mwjussfv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pejlszwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2umpzmmpa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2brgtzjfz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2szfolszr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uubgpiih.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2idycqqwj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2auweqnpm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvofmeqm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ytcxonsh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhpbnp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rlikiqak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bhbiwnrh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bznyqrqc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uhhgljwh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nywwtpak.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dfpqhiwv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jisngzpn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zbmonlmz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uhqkhazj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xnqatipm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unkslofw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iofkiect.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocqzifcz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wjexdtsl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cnzgsdmh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ospyhzck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zzapkcbf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2akbriplg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lesfjene.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hdnrwfqn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pdbjlrxl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ktlsulgt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cwhonjdv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2amafwzwp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dwsfrhgp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnhymafd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbqfxzn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ukmtbpiu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qddqjwly.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gjmnlcfa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2detsvuxt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tldjjync.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2edjeykmb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qqiitesq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2yqgxilpr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tunkwupg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jhxkmwmk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zfyvagla.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2pqgorlgi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ofqfofvq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jpypyqfm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mrgfbcym.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cxjmkuzo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2baqdskhy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlmwzglr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fzsprbai.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkvjbbt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uanlvgep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wckefpok.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdlfnwxm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2exeuxtuy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tzleetlg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2npqvdord.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltujmmkm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dmvuvkqz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpvqgbe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nzobjdey.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cmbgivdn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvnjcog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbhwuvjo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2izjxnfmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akmxgdut.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csyfkqbl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zcqqilak.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2magtqnbt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2txrorzws.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kfhahlws.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2aitublvr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kjfqiflb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yzbepiki.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xheoiikc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqfjfqtb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rwzprwhy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bzbapbev.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jcnkdpqt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hcwwhhlw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eprsqyvk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vtsetssm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fhaxicmx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hkvdtwum.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lasedpyl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xoxeeuwe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2semcbgiu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iydotyzo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zukcqvie.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hvgfteru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vveuxefc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ysieayhi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2sroexdvr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cornaoey.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hdlouztt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jctivocq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fucktkyg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dthwycwg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2romwnvus.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xmztorys.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gqhyrsrp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2svgzocwn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jeiejiyn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mimozwzr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fwcvvorq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wurvjsay.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jktybwac.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gnhcwjhy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dvscyqme.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fiojngwu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ialmcgcm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2aulgczht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fwlmgcbf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ovyqesfn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xndntqmq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbevyeyh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tvgnqrfo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrrwyir.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lmmdbyys.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qvdkovbn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wmkyahzb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kxrddjgy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odufcxqg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqibrnu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dhlirtgm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2filmdgfv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qtngpebn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xyewmuhb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2nlwshxhb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dflhltla.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ukgckxfq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dqblspmz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pttcguap.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wywdklvf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2itlqyofc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bndrprbs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yavfrarn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2igwgoxsi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hoowwpvg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fupofogf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnambumo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2byzbwzcs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zytfqqbv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jeanksdx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xugfeqcy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2doogwihf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2puohyywk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2komvmfve.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2katqlrot.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfqeqoj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lgrouxed.html


<!-- 参考信息 -->