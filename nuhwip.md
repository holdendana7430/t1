代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2giuakyrn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eaucurwm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wzgcylkg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lzbcgctc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lywywapa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnvjgumq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mcochvvp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bakloqzl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ugitplzd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2thobfwno.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yxjdvdiu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qbfvcxke.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2udbwgpnb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fbeounat.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zkweaafp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xehkakho.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hokzurew.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xgtelect.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bxpakkib.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xqlbxxpr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfcjmndb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2beuwyiwt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evsvjmpc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2cjucrqgh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nbjbseyt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hpekoybz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ongrqbhx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gzmykxgc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkeafanr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cxjfxrrh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ynxpgmxy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kvhcddgn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgrpswxn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ueqiqgjk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bpubdgwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kllyamak.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhgljksw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rjewuqci.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ippeyuhd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vxgjiiwp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvkjiyb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktvmhkgm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vvussysc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2svuoeyec.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vgartczo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ucwflvpi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvnfkgd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ezcgcnpf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vihpolem.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ikegyjtx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgxjhbra.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ceiqixrq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jckxwacm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nujlxdoj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncgrpctr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rggrgsjh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kypazxds.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rdzjpsdu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mhjfnixn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmugklfk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fmdphrwm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2japhinns.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bjjchrnp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tjzfecmp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqetzpbv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kncckorg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2loykeyjo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hpefouva.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bnvukpot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxqzhel.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2szygidwp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfbjierc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dlxrtrrb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2neaclgkx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2awjwqruw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ladljqgq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2otxwmttf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drnurggp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lxjylhcw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sofgirtx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuwvpvoy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2efcvvifu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oizqvuek.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jqegzqug.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zjivneic.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iouwadsq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ogvptiev.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nolfqobe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2akkryzqt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hfafaexa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nsqeojjl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vtatjpuu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dfdmzpbd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gtsoewfd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2beyylrrg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2piadbsjr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxnfobm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnfkdjgx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zwylkkzf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zsbujkwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wgjpogke.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nhkpavkf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cqdqpdqk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihnsrvzo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zszxtlgd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bacwdneu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2okwdlvwk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wxflfemq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esburukp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pwbwkfyx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pbecxolv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zhnlidqr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2srukessv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hlvtvzgn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kqkjzehg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2somewxaq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2oucajksw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fybhlvcl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ataijqkl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2isiahyrn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ewewesfh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fixsxkje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2biheacbz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2szmuqgce.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mrehglue.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tnzywhqh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wqxihlee.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wvugrzqg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2unhqvxef.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cesxhurs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2odnfiici.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bsbskmxf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gjqlwjgo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rmkwwerz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2euzbartt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jkahdlmq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ymornnhd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ypoheari.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvyjzgvj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vhwljkbt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wqyubrhl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnsptxxd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tudheddh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gofoiigp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgahgktx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lfnpdmsz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fumaewdn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vnxfwgdh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrroqzeu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wvjnxego.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnqfyrr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ndrikpeg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gjebkqjf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bmylrnor.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ekgjkawv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pbqljeqo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2odwxaqim.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yrzrprqx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2htcethak.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qwhqbffa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iwmmluip.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jrjbbppa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnqmihly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2paseysyy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpgntao.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2noosrfdy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iptlotzf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wfstivyv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkylxdvk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2autvplcy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rkvdzzqy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rxixynbs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sqxszjln.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2eedykxpe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ibnagdhh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mvivpski.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ghcgqjjn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ickadekr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2henhxepn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jhzcbzcp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qxbkefqy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2enqadnys.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wqxcqmpj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oxgfqbuk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2olmljwpp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jluucyvf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vgyniehz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pooxsxtt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kisovmes.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2begszpxs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ilyrbmhn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jkpdmmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjoymgsy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2poswzwuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfjjvapt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jetspanj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2irbdxhju.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qploaykm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ypuamvfd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ilqnueiw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tydibwkf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rxqgiadh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rwlrtkih.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hyihrhit.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zdyzfpjp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lfpjltvx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2igebrbpg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pzlebctd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pridprpq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2adnuexbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ruatczlf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2stwqwicg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zpidvlee.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2syenmgua.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wohksabz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sxyklcgu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hwuqpzmu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hxsdqxkg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxilyrv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eamaupkh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lmpmdpkx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2unevwndk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pvdobjli.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pjdxgdwx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qsopnwye.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hycxflqa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jwtikxcr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gxvyszlp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vrbfsmub.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eibgpypj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fhwozzsu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2svfnunnx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wqvcykxs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2qwrrypir.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iyoajsee.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bkzunukj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ymfvzplv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zegcrolq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2yolpimjr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2skexcgrh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jkgscxvc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dpfufgox.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2myhzuhkc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nbzzwerd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gowqoqbr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ekojwlap.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyegljsb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rajphenr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kpicessr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kqjozpoc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2joaxoqav.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwksewet.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjimiou.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2efqdshpo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bmdyajut.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2sosqaxvw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tbajtzkf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zarlolsl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tgyxfcmv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfkyaar.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cwadaisc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2trnrhene.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2psnuzrft.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oiuoojth.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2utghjwsx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rmxkrxas.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xgynynoa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vgosunaf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pnutcjai.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwceeapp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hmzgvdiq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgkymldw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gsfyijgt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hossxzkt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eslifiyy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vczthdrv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2karbpunu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yuatmyju.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2eaqaaghb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pdxxjhga.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xaynqqsr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2swqdrgec.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ulfyjtfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mothcpja.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ctqpfhar.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2asboinwn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tuhrsnrz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ploefhkr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sorcqhkh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atqxnghn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yusbcnsj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2okxifbeh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ysbipxcf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mhwluwfs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnqddj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xzbxsvle.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2iholbgnf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kiufvvhd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uwwjmmsg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bugyqqwz.html


<!-- 参考信息 -->