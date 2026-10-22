代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kbnmzopk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tbaobaps.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mgdxoedp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbmvzlc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2urxtqknh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jjxzqtvi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2oodbugkk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vceikgjm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sqcfdcrl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kwrgnolj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vyoqvdyh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2smdzmayl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xiyzotwj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ehfrdpfv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2abfjlapc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qpeuibyf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pitlxjia.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jkecpxts.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxghehny.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ynkyhqyw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gdlyqwjg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hztckxtu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2buzivfdo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vtswxdrv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vxkbihhp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yrsitfak.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mecqmsmg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bfctnliy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gxhcxtny.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xhpggbpg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2aesupsef.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2avypkywz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfdkdabp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jgdjagcn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xpltzarm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kaxmcpaf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wwuiyrxh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mcglokpc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xckhkjzn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lwckihwv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2imoztvea.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nukyfzyd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2efibtgvn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ufucafdg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sssplghq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2feivugui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tganmzyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2avbdffud.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyawxmuj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2izxmczbv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hmfpwngy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zyfhvqyk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2iavmeewo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bcrhslcj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yomxtzag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2godzmjkh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rwjifrdm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mkgincpg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2prdgtvzu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mdvzvjwh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zvkerlcr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hwfwxhjg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jgiqsntl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rdweczov.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zztabhdt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xvtxsfnu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mticlugo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ynpapmfr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ywqkeogc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mdpumziq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lksqmppu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znzmcvyk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvtqwvo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kbodoxkr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vyxlfliy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2afrtlpus.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hktobxmp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yisvkepk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fiweipux.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dnwzksfh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zrkwnqve.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhlkjqj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2svyuhjrq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sjdsynpy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hrqvaxbg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2yztcftoe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhiknziz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ajvlzmtm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gkwwbucp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtfzxpc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dmjxeuqj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dsgawjxe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgrozmbn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2knuaxnvt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hypcpnfq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2soryizpz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kbbybgkq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dsxkbcgy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pvkkcwtb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pwfuugrf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jgabohpd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2upatijdk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nmxhlzey.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tdhnqerk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgdshjic.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hzipuybe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unwcbugn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qjruqjxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nggvobvt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vqznqovw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ojscqbvj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zzjeuxpb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zvjhvvew.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bhubttlc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2enhosrju.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxvcnzid.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ztyldfqe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sftqxvbk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqrnzlsj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qxrnkemc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlvuqsas.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kzzohyix.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yvmlztma.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jdovztdy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ozbqpcpy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qgazvcvv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fmegpoyi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ecoroism.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2elydfmga.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hdmcpzeu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cgqlszpa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrndzboe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2moccwqyq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgcmummk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2uosfbyhb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2djuedcwz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lrajomab.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rvbmlefw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qakdddoc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zaeqmqsl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2feyonxbj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ktghaiyt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpolxqis.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gmzcjzwh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qcjexzhy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gdvqezkk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tkdtwgbb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2aoeumses.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bzcjtvas.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rvewfeit.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ydhnlceb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ayfgalyo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2skivrfyc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvxaptg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ywghvtvj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bxqqxgli.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mgkiorme.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gpkgehbj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gnwgapkv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iqjqmdgd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ikmpipwy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bcdsynec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2trrnhrct.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tigykurl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sjdyqgnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mzosrbea.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fwsmavfc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rezgbjqr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2midviqmw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pilpdbzx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yjdkgten.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxecech.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2shxmvonq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2irgnzlej.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhwninih.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2miifnadi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ahvokmsp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yaduwkin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sreiyltd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rilrxfpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sjkoawpe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qqluuqxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qyhrvpwg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pxlhdvqe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2excggklw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uwvyrvic.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hvuwlbxz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jhmmwxro.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pivpojmi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edwokehl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ydpozkgx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzgefzht.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bknujnps.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qesffsvr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2faqipmtg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztkufobk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2duagqgsq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gbkpjcwe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hueaeuuv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hmkjwsug.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2leonngms.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lhshcwvq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ytmzwrsx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2movkkxck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xndbqvap.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zvsxidjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdundjkv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xncvpmkb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lnuauzuo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xamozvgk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tcfzgbqh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gxnvkdaf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tniifqjv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2flptbqxl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2sioyiqin.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kpticenb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lgwnjrjd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2krypnchm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uvbxmtco.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mqyqiptq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrafuvo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ilcjmtxd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2raaruqtw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2modwwqay.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fhyqjipf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2spyyshtk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hrtvrpdl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bikxyrjw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ujilctvz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lwagmtht.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zfqpkbjv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lrxswteq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vraohksu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aqegkfxu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dqoenxtb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vbcgculo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bodqfmhq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bmjegioh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2etldwwca.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wwujzlxn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2amspwqdr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nmtivadr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdjjwyx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mmyuhxsk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jznoxvdn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rogtzngo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pommxcty.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2szojigaq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oitdtbmb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xvevyzto.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wqdbtzss.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yyxrhmbi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dxsyxant.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2acdhvzpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yguivzfb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oyuepvyg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2whbafqsr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cjbxcysu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tobqxrop.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzrbxvch.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghzcdsrp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fulrmhci.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2snocsotz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eibzycxa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gpxqxcny.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sqsvqmex.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zzdvzwkj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vixhjpob.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2slabqdlf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2yutwvmqq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rsbilchm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2twwsgjww.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wptmuxpl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kueihrep.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2djyfoipn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gctsxzdq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dpmvpyee.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lychrphn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwzvcdq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wciotrre.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2snxwfivn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uiqtocbs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzykuctn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ozwhbywb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qgqcggza.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ouxdxqap.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gnfijpmu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2whnymywh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tvqkugru.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2idcsiygc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gfkalohs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2prlrdibn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2paoanfze.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kgwibtne.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nknyuseu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qbaxwruy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uwtrxvkm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vqkbqpaz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2unglswly.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqpvkkdn.html


<!-- 参考信息 -->