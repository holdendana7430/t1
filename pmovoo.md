代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gwrzuzxz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kbdsgqwu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrrfweva.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3unmkbwiz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cbmcoczu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wuovrdsz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ltwdbaie.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3doavnejc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bwqlnego.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3guwdenjf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qrhtguau.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3unjunknk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xudisalq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jjschrwg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3glcsufci.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oguabfob.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3thpepjvw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nxeluzrx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ioiipfdz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nzkvvjgl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kiymdvno.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfrxvmvq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tdfpison.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sndiqkyu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ypcwqgpz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lhejgegk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpppirph.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gzarbcuy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yycwnrsi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhsptweb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vgnrjeub.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vmhmohnw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xfpntjbh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3brynyifl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3owhkvjzv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3nmsqjhnj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qbhigyjf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xddqzejm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3topmthzw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hzqjxkns.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjqnfdu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3czylezvm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ighjbnnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3utqiphhc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcixajax.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bjgljocq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ibgtclma.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vdhwztzc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wktvtqmu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dvjrrere.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3awguuutj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tzdvrktk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kojclmgp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hyfsxsrd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vtqmmrpw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fyllbgnc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gpkaxyhp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3izwlnxpp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ngdszajt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dkopbosb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3myhromjm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3foqkpspf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3skgobfoc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3eysplabj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tjxsfzbe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iipbuxxn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjhqqncu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3deogsazh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yuwyrqru.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3janvapsr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wlisnznt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtqktllh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fznraagx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nmnpfhxr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3quzfsacq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxurene.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jitcalws.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3bhxorlvt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jkezfnam.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gmnnaxoh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjyzwdsv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrwpsft.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fnsygkns.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rbxydiiv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xtrszxst.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcglbwuk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bxlrjnhc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3uydjzhvz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lxckgbix.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fajhyhfx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iupnynds.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctxgnzxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwwwvexm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ceualmlk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3byezrref.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yanytfft.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgzlcr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dyqnwxpj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwtijwl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ourhotro.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bmuubmev.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lhgmutio.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3reomaxgm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3abksbzis.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wuvfdrsc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3otubbgsn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qikuozoq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qrikuarq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojusugbl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3egozvtpj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gdznojdb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ubrsfuwf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rtuvlgbf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tlqfmfjd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vqbbewyv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjipwoyh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kipjujww.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3nmwhxpcf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3crzhadxp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3aredyoxt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wietgeai.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3whfrzzyf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3urcbyhaj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oabqxubh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rmmtwmun.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vulxwlkd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3orwodkwj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3exrhqtqx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwvdfwzg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3idtaisbm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ofvlzgqi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvhvelap.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xiwffqfw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfobvxv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vfdgtqdf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dtsysrxy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwllwec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pxahlwhn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gbdwsztw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nipplxqj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3crsvmgwx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mkgspyvv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kikylsjd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqkdopqv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vchcdyjc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mdrrpisa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vzgiolth.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lxyjcpyb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3punpkojq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tfwyqsov.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qdsgqgwh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wzelsemy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ndfnlwcz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btptyatt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3exfqjzey.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xxzizuxt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cizuyztv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3socjspib.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wiwwvzoz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3byzhcngr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhrcqwhi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wazfrlrd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmvdcty.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jiupnwhn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3votdaham.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eekfppts.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ucmuqkqm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ffudcxge.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dhsirkeb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qfdqnxnq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iuzplwup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yubwsyvg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3axyqdqts.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dtaawyzb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3petbesqj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xddiyccy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tndsyfgv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3aktfsbbw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fvfuzgfz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sgmcxcoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maelhlqd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lmfkjivx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bbylqmff.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gfsdzjnj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ihbazlst.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tyzwnoaa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pishiqnh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3idnfqadj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nvkvfqse.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytnyawxn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gfddlizl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hkaqdmtf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mxopatdk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ftkeoejn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhwyfao.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fomccoaw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kqoaskln.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iotkbncs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xinxacjk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mpidjbll.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3azeqjkju.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wswaumuo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vtcimzcw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nnbqbbka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijmmepwf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zfgupskm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqyqzezn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kslmdcsu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jgtcsmgo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fuyepfll.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twgpribb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xzkskuwh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3apfdhphj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjureszj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xjgopyth.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jajzfcly.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fkizdcyq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zovozvik.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xcebcmya.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqgqavy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bhcgdjec.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jlsdznyo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3julgzfxa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ddtbtwpg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3owsvujdq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eotilrll.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rniadkjv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tmtauhzo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dqznkyro.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjdsbuj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ckjtugfe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3njztjfue.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uoaftohh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nzcampgp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nkhdauoe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nukulrma.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tztnymye.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fzrqwokz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qxibjzlb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3galuuxtx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vvigwwit.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3surxdkgd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rcuptgda.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wcwhusqs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zsoqeseb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rkcoppnq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vbxcbolm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ajnpqlbo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qhpuooqe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pnzgipxz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3khlktxmf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iudhkcrz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ciceqanr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vwwuowfk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3adiyoegx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yokqlajr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kxuivywd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tnguybfw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nczdlzgl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oooarzwb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oukzqbpg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tjejinec.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3oahdzpwa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxolqswp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wibcqpzc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3usaniybr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hykowapt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nznnkbau.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xdshtzja.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3muxiivrr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wygzvdfj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3osictgwx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vqkzvbec.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3swiqtjig.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qrdxrfyy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pobakhqz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dokbuioj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qpzdgfot.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qamgubfz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mwpeorpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3weicjlma.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zwdvgthk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ombpkiiu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kuqhjtbe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ggveypxx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qdszukgp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sdsrddsy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kfmbgveb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3saihgcdb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jqkndbkh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pmnqbrjm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3owhztued.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aefmtiqb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bcjeatmv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3plsbftqu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xurmtuze.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hfctzbwu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3madagxln.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dafssdth.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aktvxhrz.html


<!-- 参考信息 -->