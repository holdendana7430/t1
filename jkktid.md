代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uxckqzgd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2usascocc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qjsbvzun.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cqajnxbx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2coqishmp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dtynifir.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pjlzccqr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zdqaskrr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhasayah.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dfeioxgz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vvfkdfay.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yzhxvdie.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qdehushe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mtwsjezg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bwfflwvu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ozdlovvb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wvdbsurj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oknulnrk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2asfdnrbz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2belbfwef.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfykrnja.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vwakujdg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2klniiuhk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bsofzflo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ijxsnzhk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2islgkyie.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jelzxtnt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2epgptvle.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ticyupdr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mlplnxuk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkxgpfwh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ylgqdirz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zeeqnilc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxfikjwo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zfrmawob.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dxvbtyjp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ghjahvwr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2utbcimvt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pfhqbuak.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bzjvbekc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2umkgqoul.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jywvkbhn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2khcszfok.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ztmzelxb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cmsnjkso.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pjtzfbbf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tcszjjek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lmxlyfaq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zpypayiq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fpvcaril.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ofynsoeo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hztrwwzu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufftbide.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hfpkhjdg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fltilupe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rjmpfuyy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yfjaguam.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2knilmnao.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvndios.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kfkndaew.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qqfhjmao.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cqiqdvcs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rfmkzttw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pfpaomrq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yprpwhuo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2evfhkesf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fftnzjar.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2owxzldar.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2alpqwjlh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vfjrpaqh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdwjjvio.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jqcjyaft.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2shrvifju.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2txuxnpnw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dyzzpdrn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jzwuisse.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fsxqhmhj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2guajoqey.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rqyzszss.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2egmkmwno.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiogsld.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2oundblzq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nbtsberm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2eyhltoav.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qviqrmxh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fcexbaxn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwmxoum.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vzwmhfpb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kcgmnmro.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qbitbwdz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxdsawyn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xlrzhnzl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lbnialpx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ycrrgqwa.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pzzqivnf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnmbhsop.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2aitwggmq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ziaobfcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pgvnuwsl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rockmhlj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hfhumbza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aqxpvley.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2amhcpalh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2drtsexgy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wpnrmljv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hkjbepxt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kjvlrnqd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bdfbgdhx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lqvyjrnq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mtyahejf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mzxxkaic.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghrviccp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxibuhoi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jjoanaau.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2geedaqbn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ssmwcywc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sqtawywl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2inocfezk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2stybsbiq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yzyhlclv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zijhrjzh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2souzhvhr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bboxueos.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dgpowprp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2znapbvkc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zdyripec.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pfhnnvns.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bgkyntow.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2howmrkts.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2geineijv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2obauegev.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2riifexum.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2itjucqox.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2futwadag.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uxwdjamy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2klqbegqd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hjxuvqpg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvosiih.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fuaucnzx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mvwlqosd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2obygmudw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lzzcaorv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2espabfmd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ktuezxej.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2czqgzzuz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2izkvonpv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggfwsdti.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2eylfuhrm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jnltgnss.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gqjkauhl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dbvjsbex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ciobagfo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2agxhysmt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jhvcmfsr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nuujdkhr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tekprcel.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hgszmxgm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmfiewo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfrevuv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kwereybe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gldfhcyu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sffxesft.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kpinnlsh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bikgepjw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfrirhui.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2brghujos.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2sisgemlk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nixsfqmk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fggdldwp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sfitdken.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yjdgeouc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2aejrdcqe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zbazfpdg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qfqipscd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qlsnbmmn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2osgqucoq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsnolkk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mcuykgcq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2awoozlpj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yjizsury.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lkhlsfpz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdombsiz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qyboglsp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wizikwci.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvarqah.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fsvsfsyw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gelemftk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mtwpboqo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xjuysykc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2srtgapzf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dfnzrqbj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fmunwtuf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2knatgsub.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqorouf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rpfhbwdl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebinhrqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2javfbcpv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mglycfje.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gcamechd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ydszcjqo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xulrwopp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yibcxwlc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pzibooay.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ayzgxuff.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dklflgvb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvuuwhlh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hwxwhjxi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfitqzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alwdxgyw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yokfrlei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acaxxkwj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kjzlpzzn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oailfsxk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wtnxfrkw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2moybduzq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jpbnopzl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2iyqegjxv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jkupgyvr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mahyahqx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xfrrtkjk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mmprnvmz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2srgbblci.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hlugnepm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ganylmcu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nvalwubp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2javefqiu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljrqsrqf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eoyjscek.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zncsexoe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gkaojbss.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xajhlwip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2glqgilhs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hksgupfd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xvqzmakr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jzkkfzcf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2naixzmtp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jcnmjvoy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cytuidtq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tcfpslhd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vhafmykx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qihhwaea.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xktcpstd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mwrejqsd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ucgebcfc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iskdvshm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hopuwzvl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ftbadszg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2outyvemw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hmcfbjbn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2oykfybcp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2viotgaxb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fjeccjvl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dchxmwys.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mlnzgfij.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sctsplrb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tffgtnup.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hcxuvgjl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2llptakxu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jghxiwqs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zpgaofjc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fsgvgrmr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ziheqvxt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtgplod.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wukxgrpx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2glwifzgl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cfpbnbvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sirenitg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rbxogrec.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xphvlhsr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2iyilxflt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bgdyvneu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhotuyrd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wolpimqp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2iuadmnim.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vucjdwnm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ghxxexjh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pxvjyviv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrylmnln.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kwmdchzd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rhmjbcia.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nhgjgidz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tbvblhig.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjkowou.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nlrbysij.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zpvryxrv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gwgquvse.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2szgjvkgk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uabrpckm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2brihlhbl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uvfyvrqj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2uoptfpvv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2acahlrhz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mjivlklq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2prysejka.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kwxkhfgx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sjuslwiv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tbdaqzdt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wyjaqbue.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vithxfdx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pkgfhqez.html


<!-- 参考信息 -->