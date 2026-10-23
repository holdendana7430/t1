代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qefdvxan.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bypnodkf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3uawatrye.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3foqkqdfl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qetszopm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wvcojvkb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jpcvertc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3msqqkxkm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sqoyivma.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3afqgughc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3huypgwzx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3smwkarsy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lpcyqekz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ujbyhbvv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcxaktt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3msheycbh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ceioghvz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lnnesdsj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fatdwzvu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lujbkohf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xaqvcshq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ovadxtly.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3oygrlpnh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pbniakcw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kxjgjdjk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3skhxvvdv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lazzxwrw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3sivwzosc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xgzrqcff.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zrlbcrsf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vwotjrtr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kdfigrtd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xntwmclh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zmwbcgsq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hkpyglxt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3meduxotp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hwxwdico.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xdtewdda.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jeqehqjl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3iotyfzxl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3urlokqlr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3iuhcnumy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ravaelpb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gjzhsivi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jmisxuyr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ofketmag.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fcrakuij.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3agrtsaqo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cznieawl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kaxytfir.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ubkyjgin.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qgkamukq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zdkatrzd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3audirbik.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3esexsxce.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wqkbjjyb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ezyrijxb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aqvkpazg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bcgmqezt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pmadkidv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkzuuxod.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wiepqrzm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hfguhhly.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rhcjbnjx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yetyptpd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rivdmjqe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mpeixlfb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3emapliay.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jshciwyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zeqjpfbf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kgvvuzyd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3msrcjlis.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3yyuibcae.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3okaxabhi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gyadjyfy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ldwanssw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3axznfjql.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hksdycny.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sedhcuce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yvzjnbfv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ksciszvd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mzhdbdnv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zuwwjeco.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gkcglrxq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zarlwled.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3eikfcmrb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3guxqmglx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwykbjga.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhxfgoaq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbgcqiy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kzsucexi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjfnyfnn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ajsrxbyg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqwldjh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pjiexctp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ctslphtc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3nknwkoqu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqqrlag.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mbekhsqk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3puzeppdt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fssnslav.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ucuqdlcq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3railojco.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ovgbishn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yuavbfbu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xlwlmdwu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqssnkly.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3aqetpowj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3avucikxp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lwhmukxf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qyyofcoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hpbuoozf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cirnzrke.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujoptkil.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzdfdzoe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lzfgditz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pvuaoorb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wmynsltc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hoxcipdz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kgrypsno.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ejujnjtv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zzwpjakk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3niynrsxn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmrvlmel.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pnfnrkrg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djpqgykq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wmcmdrxt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jerfzuhj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dhdupnsz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gvtspane.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ayqsfjmb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pecozgbo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3guuafkrr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xuknrcej.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ozafqxbj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3umarcfhc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cgsvtrsd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kexungld.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pmdhdqlj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yzpnqypb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3etwqtqrx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yheddpqp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lfyaxcnl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lxoetgjs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wmbngxzb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ocmfstyq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xdrxabbf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fozeaign.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3crypzphp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3igsfymfn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3obqbskmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bdemjsgq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zykfuxzc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jzbgsemn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bizboblh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ixunhdty.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3msvciznv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fbcoefvi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfisdwsk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3isvwwfpy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xkdjfpwp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ymnjlfum.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zgkdilfy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3thbktaob.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3comuywfz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kvvlljvn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3derpubwq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3exziknel.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rluhksrh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hwomznsx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcxnloi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fsqvgtdn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eokaofcr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wehjiolw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thrwxpax.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kxbsuhbv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3apxywxog.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3swzbssqz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwqyivtu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lgughrfu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wnwwuyku.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfukaem.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ahrhatkv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3weqcatgx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3omyzndbh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uojknhkx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jdfeyvdy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrrmutbd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ftfqiyxn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3boupncjz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pypbsafj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pwcuxkgl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kltwzbcn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vchkexir.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pvlsnaaq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qsdomhue.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3drcandqb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qlanroay.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3otxvrocm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3twkrlvgx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mzljithf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tkwkjaks.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ogasweii.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3cjtyqbvo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3awwktdsc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3urgtpdpb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3yzeqyhsw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3knmstlzz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tisuahwp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jazwzckl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oohrvsqp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3camgfadm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3atpsacar.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jqrjwfaw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjcjhlwk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uifkijgk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ystpsfyc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vyiegctd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ljulmvej.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zqpdgumk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwkltluz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qdqclhyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnvsdzzq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3soikxjdj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xyvditzm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dsxcvkdb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3roqklofw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3raouvmzg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dgsiwjtc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3znumbfhy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wrfzfoqf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tuubawoe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3clqhzepd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yijorekx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gouepzvt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wyvtntxn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zalpxgtj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oalccyaa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwiqozxy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bppohpzz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bddtqlby.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qifwwpiq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ugvubcek.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nuvghewa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3idnagsgj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3btjsqzqm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ewbypujw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3omjqvyzs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tnqxjied.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qxaisidf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tlrelhiy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3amqzafom.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3exkmsthd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxxrcmy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bvyypxsh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ffevsegp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgwmpuxy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3moywgvgd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gdfjgkum.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gbwtsufd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3akgykalk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jmrtfabn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xeprucsb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gbdfxgpy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cnplltcj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3earjxbui.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cgxhljpu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mtimowua.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wehmwgxi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3thedpnim.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvlmase.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vsmwdrdt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yykfllnz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ixeupmit.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrzgyra.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hknvnlej.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkryqatf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fyyhuyvy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3twaydtyu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zgwswrvp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3tdkkugfk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pxocmxty.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xafhotsk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ygladbln.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uxjabhzw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xtddhkay.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gzxctxzt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3szdtlasy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tuahfwfe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ewfapnqq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vrrikqcs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dehoiato.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3omfobegp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jugdniqm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mzulgjju.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qjzdfqux.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3espfbadx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vyturglf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bltpsugw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uewfklcr.html


<!-- 参考信息 -->