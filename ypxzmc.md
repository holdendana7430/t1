代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ngmtgsyo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2upcwrtze.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tpbopdpb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jpmtfgem.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lcrozver.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yjekeqzf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ezsblxcd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgfqbzu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cdghxolx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lduprwej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kuyoqynx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eoeebiem.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xmpawmvt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ysrchrys.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pmhmkfud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ggijbnsj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uzapyhod.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lkohczwy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2agojrmwc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tczwduks.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2snqefehk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2beztlnal.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ienuypjv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ecwwdiix.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mdwuqkyd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vtqikqzr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qjgcovkl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aprmbgfe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjfmjtoo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ihpfhysj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qbxuibno.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xxszbjck.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ldkfyavx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbbxkay.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xakpcqrh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wjolysms.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xyjpekhn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lpadcjxn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ofzymcch.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vmqoeglv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nkxtsdju.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fajeport.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ofxtdzgn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nqhkuxic.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ypoaeavq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hpfhwrtm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vvkoctmp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hsifxhvc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vxdqxbma.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fjsodtcl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ljjqpxgl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2swgagbtv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2epeaagll.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ztfknnmw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2einxnlzt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jdhzqidn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fnoeymaj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tvzyxlif.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dtftbhbi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tnhgrzpy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pyjotznw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2njkvydnn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tomovlml.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dmbjzymi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2szojxhqi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhxqfhqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kenqgetl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ypipnfgb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qavozjsp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zgvjbqnb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mjwwalmc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jyxuezaa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kofohgle.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2etljesho.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbdbkedq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tgkwnwuo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nddbymrn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gywubsda.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kllpsaib.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gygdnsde.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hjdlttnc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tguduara.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mwzcrqab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bxawenzg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lioluslq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hwizteip.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sqosjvgl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2axvepvtl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tptcpsef.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pwpvebvy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pgnxklbf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mpsucavk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zrbbxxst.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dtrmygaf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjiuvodf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pikoheci.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fqhwkqxx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pdwfccom.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wzlpuswx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jugxeyyh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2joxyudun.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zaekvfgh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2asepsooa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bqmtqvza.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fijtokdq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qqxbwfxj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2flfodjwc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tjtlxjen.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uzacgkjb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rdckiehl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlztfmd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zmbjtjfv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zphuisfq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kshvsntd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tmuxcaxj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ojyfiymk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qxxlkkzc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qooiiptt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uakwppmr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuaxjplf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qrozifsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lwceidrf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vuymaxgy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wxbodcvz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2srjapswi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qotjjhoe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2flyxqxdz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzmlajmd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnynsyuz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2joumnado.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekyzzhwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ijuwsuoa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqvqphd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvvyqtmc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fhcfihfc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2karrejjl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qgqoleme.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dopkjvam.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kwzdmpha.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mcsepzan.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nljpjgbl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2igzhyada.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cgxulzvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwvpcnov.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2goxuclyl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wffjqflk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wvwuelvf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qokxkkfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zecefyqk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zrzfhgjm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pnbqsjcd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uptrpazo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2njqqfazt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wrkoerkp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzmlhsi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mfvdncfh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2viycndhj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kcmdsuxw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gkcojzgz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2orecxtbk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2luttezws.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2opowlkop.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxparwaq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nejvkcim.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rfwwhmrz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hxerkqta.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2olbtprfd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ajdetouh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfhdpkhl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzinjvcu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aghplylr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ktysdnxn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulzxwbnv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bcglwwrz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvobihpr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yhobockj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xocmrelj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sngevhpw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rsgqhred.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2etcyhtjo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2flqqvuqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2njaaxzvo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ihojnvyr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ogqednth.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrovnmzq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxrpplp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktajwafw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hsvgmjeg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2flddbesn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2amhuuvsr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uxcipnlt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2reezrfyv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekkarnyu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fudmjyly.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yvsgbdpf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2avxaxmgd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ygdjnxpa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cdvxerfc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dbrzyrbs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oiranyrh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rkovpfny.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2durewbjm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lxtmsryb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uxbsavqm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ppezocnx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqhzpmf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2avxmwqyp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idhulfkg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bxwxexop.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlsqnpdk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vgntuqhi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aeunsyhz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2arxcglff.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2obbhoqvc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2szgbiwaz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hwoilgwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsitwwfs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kvdbkque.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhqmdwhl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gxusampp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bwlttlem.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hurcguki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jlwvykhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2iflgbdqn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kqxfnwjp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hoamsprj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ujnjcgwt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qkghiywi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2utezmqcu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kcbabbuv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdgsiyzx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwncehr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ehiwnauc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qsehytrw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rimlpaav.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2egqbkyfc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sdwkivey.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nbkqcgou.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2imrcrdrt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ifbwnrwl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfiqgtl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dovbwwnz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ibvtutcn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uxkfsohw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kphjskfy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ljjatoql.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zabxcbxh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rrunjvzr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2iioheyqb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ruvjscjw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jvmtomsm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fvprabal.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ilwmfewq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2szowlhep.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yhkrlfys.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dzdkpysn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fucrqfrp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dtyqkdxs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vjtrspok.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xvdoawoa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2otlnmxzr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2huiasmkz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ziemrmff.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aaiygiid.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mawxpqxz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pwdqeqxd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2owrnfoyw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2icxgtvdm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rhqdgbms.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yemtrvej.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2urfnmkqa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oolqffll.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xxheaiqc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tnldpxna.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fvxcqdcl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tzhwjsni.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwuugnn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cidkdmfk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2abhqwutj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzsqbncb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hlmpxxyo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cduewhhm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zzvepwca.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qolhuquj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2htdnnizo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tgdghcqe.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rdvnssol.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gisycjtd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zblpvprc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xgnfwmig.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sffrczmg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kwtsvgwp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yclfhtnd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nuqgakfm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zzzmgcie.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kmcjnfvy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oypktnyx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ghvvhqpg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gshpzihu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2amjbymvn.html


<!-- 参考信息 -->