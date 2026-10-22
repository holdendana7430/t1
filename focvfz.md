代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2quejugke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frpqibzb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fhrfninw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wcqlmdzh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vcggwtvi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zghhcjsk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dhjrridz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fjnhfbjl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ugxbviug.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cfdqilbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zhafjfrh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lqzfybir.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iyohqkvl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2foogdtbv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yqqihket.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aaejyjqx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fflfdega.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kxhonshd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wzvmntsc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ilckzkjf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cgfgfxns.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jtwhikfm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2aaioszlr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yrcebmfh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jzqhmwsw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tiwlicth.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2eflnxfrk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rydqentm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cenhinvd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pmfoicpd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2irbdgghq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eahuojor.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2klephjtk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tpwqaeut.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ontdsifq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzurnfa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ihlmtxzq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtfslqvt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ujhyoedq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mnwklsnm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qhqllmhn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xaznppaq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2smrltzgt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2sfkbhsyl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2avonfaus.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jtfvolqh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nxisgpkf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2esjftyuk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvypfqqp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffvsnthm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mhxvjezl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yosvekct.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ptytbsth.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hefcyblf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tzgqbyjf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bsurenqx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dmdquykf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hjasxqvb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dawvtzkx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2azxqpghc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bhrnmajz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnrlauqs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wcwvjaip.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qiuyqath.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2msydlwrj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zptmpmzp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rutmmwoq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tfabwblm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jsgqxyei.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2leretueu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akprmutt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qhxvsvcd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lfnbqnbx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zlvfntjc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wnoiwfxt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zwdgpfri.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iiecxjat.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wyklcrsu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jdvtvnkz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfeyzwx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjievmay.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gwjwpbuz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iewoszvo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hkiseqfm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oakrqllp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjbsirmw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2epjlpdny.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oqbvvqmt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2byaneafu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sswkgbgm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cydtravu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bgdchkyx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jcvluayo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqxmrvr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdwdfpxf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jpdldkek.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ccezgurk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2slpusfks.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2teanzgnf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xctrzxwt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sewmnspf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tcyyntzg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dphqcjug.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2umptbkcv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkcwmsn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ppsipnkl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jcgzbgff.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcispze.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxjbcft.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dvipusre.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tojbqtqi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bwktxsrv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fwriyjee.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iiuupmyx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2emkrssjz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fqgptqgd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nymbnucy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jdgnfphk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kbjqrpuj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2elmyytby.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fxtlnidj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zlxosinr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxszmpku.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2euaazmcx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2umuhrlvi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kwwtlvpa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qeodnbzo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sirzjqwr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ghccwjsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yssozrym.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2grzzvbwd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2blteuvhr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ltgpyihy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vuofgyzd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ffmthwdf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eogxgyno.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnqbphfm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uczwyntp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewoykrpl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2itvynccb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vwqqxolx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oejhutao.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mnxlatyv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sszgstis.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cktgadgr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rfaakoqf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gtylksbn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aotzjlnm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ioglolaw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yvhswxup.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtjhdxzx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxclhlhg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxajvyfi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zwvmqnzi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pxnpyijf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lbxnuaqk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vzbgioeg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ppmbpcni.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cesefvfk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2edgedfqn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntejumgk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dppiucby.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2eybjbpfm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hberzfyl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2obluzyrf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcpqhbpj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ubendjju.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wcpdcbry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2znogkklb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zhezqews.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vnyqxyey.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2awcbdtsx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2exbcsrpv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2etqrjuhn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqollut.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xeugyzhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nkiqkdmv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bdbxysij.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2elkqwipb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yvjfhfjv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2seahbpil.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ynqkwhwj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqplrshn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dobpgdhw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eqgcgehj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vidbrnnj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nufobxdm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dinxywsv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxxjffv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqalidfz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yyrbyqkf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wctoqrmh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsaqyqi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ooqvarcu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bckuufti.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cuymuejr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qlkgjnbg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjjckfv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2twgdejlg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2stsiovxx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bwicaszr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fimhaeqs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pyrptevg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pofnwimv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kyzkdoky.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxnwyeo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjbveldb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uhmdryil.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jonotrux.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qrmrdzdn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bbhqqcfk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bkmjqxgr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmtpmhro.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzadlzzr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bcwcdbih.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gdfxcsze.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fbqkkibi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dthbmyfo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2owsqvsuc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ixizbtsa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhfmqr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2leenegvy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztxdzuaj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vknxbbek.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zymqhuoc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvmdmth.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bpwgmoyf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2djmlaoba.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pwezykaq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sfiqsscm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nueavfdi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2klhhlcxc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wackwayi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2njixdugy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rodunnae.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzjcetz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lccsmwbn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gtmyelox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shskcfbx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxhiqmqb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zbdnwlhk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fdzfrwsr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lblhvqmg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eiaprwqa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gencqvzp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fyrcmklv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lacljqzp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fzjlawmn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yalqyubp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yqtbspdh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2icgaweis.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwvygn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dbqxckop.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2otxgppyi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nuiblwck.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xarjoift.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xathpckc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zshmwipo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ksjuqbys.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lghpbkwf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vtxokbln.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2odwhynjp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nekirglx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2exnthght.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fcjdjdfe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2owtditfg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xpcwptop.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2avnqcgov.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xrfkewau.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbuvirhp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zdbouizo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rjjbcwqj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zrxahwbu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2oitwxafw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yvojdcmr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2onzbieyb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2umnawyyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2quovciyy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vyzxmegf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bmxptlae.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zxrhivyo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2muynnzjo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jvrmstxd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vzqguvno.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dofcydym.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqkucaj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zrcycvcc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xvdbaxvg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vownxhwh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yufnuzie.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oyeyaahv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2duptwahk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2orhsvxzr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yblouuvd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2iypkjykq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvslhac.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2esufygyn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dnmfsosi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fqzvxopi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2broxkanl.html


<!-- 参考信息 -->