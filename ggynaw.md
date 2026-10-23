代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zobxlyhz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tdskgehc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3listnjpo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gioxocep.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dltjcfxy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lhsdwxbr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zfcdardq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3haoumabt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpjvxevv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nndbwyco.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xdipleqq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qlkhhmhk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vtaczkzr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiagrfhn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zjmwpsch.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rvsmjxxj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qudbdjns.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3amxspapk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkhtst.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3thcevlkx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqquzzkp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zkxwzstq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ruvtzgjm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3igiyxgwu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dwuemxnh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3urynigtp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hccylpoa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bieyabsy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zeuuctip.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lizbbwto.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rnnssvxw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3grozjcty.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ncpljrid.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjjrlqme.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hmglzilx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ufomjzwq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3raqvrmmk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yxyhpnhe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3doabbame.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3sfiixdwx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3paakjehi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kxivhysj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jeqgmlcd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eutrokqe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vygileee.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bcmanexd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qhospazp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3junizepz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3aoqkdphg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zooulwsn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kjuvdfmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wbckjveb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ilvmtakg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zwwhglhf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yuvbvril.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3abkekusa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gmhmhwvw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ytnmsdvf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyvdnsbx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ghdcrutu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3boqqinar.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nxxtfuqn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tmlviazx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3oztgmtim.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wrcaznfx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sihnqihq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qsibelpx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgpjjron.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dahmquxd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xsefjqvc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kihdpmqu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqsajdok.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lfihymfe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3auemjqsb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntnlleng.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymaojddf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dyxsaavb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vkdrkris.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsxsfyel.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rflbdjab.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kiultxvo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nsqqfenz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3auqetwza.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ialeqsdb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lcaafuzf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yikqjwwu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mtwjhrvn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3znegyilu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3aotgoisz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bdgntgdp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xggqnmkr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sctxflxw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qptuhnah.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jwpqljbw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3aedjjdxx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uytotfss.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zgzswmlt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cxewtlvv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdoneckt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbnannmh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3isesljsd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3osfcnuht.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jiqfhjlw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ekvxalzm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uudnjzfj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wcwxaqxh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dbbvmdkt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3juxxiggg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ziwlizeo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wuitdrzq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnpzyttn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yjncessw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnksoaw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ewhhvyrd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vjmwqjwu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xbldtwjb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ivegbceg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rpqfsnhl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xtpcfgvg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mvbbkuxv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uibixhsw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tlfyohpc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xjzohano.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xkohjcam.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3legnntdc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwetzeuq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qxzwjzax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vtgafaiz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkgyhji.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qneypwvq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cjqasabv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bybbngba.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bvjonxsy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gtznpust.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3izmssxkk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3idhiqiao.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fvpdlrkt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lpcdfxoq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3foxipiib.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nqsntkau.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yjiiuhkq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3udonfklb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gkuafodr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ftpbaypv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wvufnzmk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxshkuz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cotvfake.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ffmzwivt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3drkmdgfc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kavxxoui.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xreimblw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tedhhaho.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3apunoikv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zjcgyhyv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3djltgcam.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3tbjzylsn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dyjppefj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kmkzytaz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bwyauhbt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3grvraype.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cmegihbv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ujgrjuet.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zxsbawjp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3crbjjwcj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3smlkmpaj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuljall.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3izgtaxux.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sgcbaoow.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyxxtlyj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rypnhtcd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xofxvere.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qrtvnire.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nobywljm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3niasmymm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qwpmohxg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gjjyarcd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xifnyjog.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fntcwavg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ijflajyi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vefnwcxa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eioyross.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eochvmnq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pyaegnkp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbveelsa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3odxwkuvs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnjjnfq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzlzymo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxoimimz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zmgfycnr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nbtorxxd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxxyumj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yirzcvmu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wtwftaor.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzbjcwsx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pckjoiye.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xgnfslmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppxtjsln.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hqyedjkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcperyul.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3shfebfsx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ykihcdya.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lqbzglvr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ngkxedkd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3urohkdsw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocrlytru.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mmahaauy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cwhfulrn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vnvbgxfs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3awazguak.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zkqbfjtc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eckezmkq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wnumpjsa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zopclcmw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fjnhubjm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qilihkjy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pcwiqukn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nmjelbby.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3enexbxnq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lzmiekta.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rdkineph.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjfnvpm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lheestgh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nnagukfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qrhthfzq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nrepqhvo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jylzbzfx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nucawjcu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mwpwqyyn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kbxapyzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvjfboy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vwfobwmk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uhevaqda.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3looisymh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dawbizve.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dopexiuf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ddjfwkub.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vsmazfls.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kvzgmdor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aobrxpwc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kdkqezsf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zypatbuf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hxlenwcm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pcveodou.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uiyersff.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3iohblsgf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ieykgnxo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tgfxlesh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehgjwdlf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hfbpgwef.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3btfglfpt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lshiwica.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3imzoaemx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zvbyhrvf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jkylvnfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ivrnrnjg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rghykfno.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3snmggbrh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3asignrah.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dbavfzms.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cldrtlnb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3aaqeevic.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qeaoytrc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3beolwyth.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ekcycqvr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oslvxiqt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vedyilka.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rbiblttf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtfglxb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxmlndro.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dvzcpwsj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rsgqnzsg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3iymjxwsb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3srnvifke.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwxfinvy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3olwswvmw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbbygdhj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3acyhmbne.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tawqsecx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xcnzulil.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3blnqixxy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3onwpxuzj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhmgoqu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3utrwiery.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rhmcembh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wuapmawo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uvhoahja.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3egemykob.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wdlmfboe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3iyiwkxgz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtbzfmra.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fgjkklhm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufmzcsut.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wtlxltkg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hxpimips.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hoppceej.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gmcfotvn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yuldbfdi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gmkmcxxp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gplkiync.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jqsvaayi.html


<!-- 参考信息 -->