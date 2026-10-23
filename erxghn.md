代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3suasrgsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obhcevdl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xkatwery.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cjsfxluc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3obhryhyq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zznaptxp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3joogcrfb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iumkkqwe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ittdploq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cehwjkur.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vxnwnbdf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qzleibyq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mvvigilb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3agpdzege.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3okyfwsox.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qayskmvo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3gahqzwlc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rgamqcct.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mtciljfu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3scxoncue.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hvfxaqtw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwzcmqgj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mgbyeiux.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3iqsotfbp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3psszsckx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3efkltnhh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mophekcq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nqnoskrc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3klaugejc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xhgzydza.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nsxsvwoh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dbgitywt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qurvmpjp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uorkawcp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ikvwrcyn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnhdpbw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3knflfnrf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zorotegk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3reippqud.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uwlbeubl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3apsvgttg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pquxitbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jtombbbl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qligucmb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rjtjqfai.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vjddisrk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gjeszias.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3msniospj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uoelcgkz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3folbignq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fljmymkn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rcrbmtwc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zahoffic.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtbdurku.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rahcnncc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ykgodwyx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ytmkmtza.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3htnggmhp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3frqyfaua.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvtaqhi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yufcgriq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wgmnuinx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3htvwgbae.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wffcdpql.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fnklxizm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ccyifvrj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vmfnvivk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fetnlhmz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ybppkcss.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3eartpaur.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kevddrcm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xwjsmamb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jqzdyzlr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mupmzsqi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ylhcqkiw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vmjvgcrj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3azmmnksf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ydkfbcfv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ydjljlpv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dijvwozw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlklsua.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dslqefod.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dxrdspba.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tgcjigsd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3irtytgyv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewzfqitf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlwmvpb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zjrttwmq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dszvnpxu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yudvuzsi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ohxducuj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yemdchzl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rvcsqqlh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ctkzyzoj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dwzosnnj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bogoleth.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pljmcykz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3flayhzmv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnfamvw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gsnaongj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kmpivmqw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kvedywsq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cuupktoj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xosmedoq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uazmqsrs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xfztlkhx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ohizerqq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hwbtdcvy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ipazsnzh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rgvyrscc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3piohbkpl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qmenxydp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3plxetksh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3efcjlnwv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujyylodk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyuzetwn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bkcpuazp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bwqghbrz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rujdexuw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bnnbrwwu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ifzoxajl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lecytgmk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zthatajl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxuhpca.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdvttqmv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wmnvibpt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cszzcghh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftgmfjdr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rvvsbvor.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3evasglcc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lppzuapj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vdhnaiib.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pvepfkbj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pkbsipzj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bblxvqji.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tvvigbel.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3urymgwwp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zchvjqnu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvaclhn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynborjdn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3infmwjai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tnburlal.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hrizwsso.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bwbmqvvj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3birbytxq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tmspefjh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3blyxyahh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jetfvvit.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjbteocl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gswpjqzx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xvwrtdlh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vrgjuoea.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fncflusq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jejxuekx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nrrizliw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xfpnrewv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lvypghij.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hiasczkk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ptyuhgmf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3trnmqlkk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ygkdkndv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cfxctixf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3krlsdvqa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjjezimw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yvwaodbg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtjowjm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3labqfwpy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ehtsfnch.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ubcutxbi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3sqpziinj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ofoxwzlh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kppnplqs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3djsosoeb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bfnwldnj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncncevzc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hpnzumbd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rsxcphao.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jizzjlvl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xmykjfuu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kwcfsazl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zqdfwbxo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kyjntnbw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vijixeui.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nzkhylbo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mbhzqgla.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnimod.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnsoald.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hubacccj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjunubyo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pwdsuepc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3twstwqti.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bfeyacfu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwthzuq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3giwhccjy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ayfkqffj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gryqtpbf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hctnerjr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rypfhron.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kcmhhtoh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3glrhxbqq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3irophzls.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ysfpifer.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3eggkoken.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfccbjf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ryuqilak.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jjgofcxz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3plsgzljp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3drdkgwhc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3chdjigwv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lobwxjvw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xclsaekg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymqbgzdz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3edrbtmcq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3irjcroyw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jsffucdl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gnbpwozz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3clenawuj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3eezuyrai.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qgbadbrt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3luvnddxq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3svwoldlk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhqxcl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3imvsoesq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxzjxyv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sesndvol.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dbfxbtcg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3koeklknm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxkuhwjo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pkfilmfo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hapwjvtf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3chtckpmk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3arizdnbc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzddlyc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3eatsvqgu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xklfvvbu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ksyeayqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwwekdcx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hsuahsib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdzasmrj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3auttyhgy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sbydyznk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cbbvyibi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yfkbvzly.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fpjuabsk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3azmdozbm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rvastnng.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3clazjqje.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qnrcvxhn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bdtdpgik.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3khkpfwlj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rogqapjy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3crjtgssz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zcyoddhm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3okteztbe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fubgmzbu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wcqkbyli.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bzwisfup.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cangkuxa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tzwypykk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jriiszgo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yxnvbevh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rgloywdg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3apkzkzxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mgoslapx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qsydhnwv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pavmhjuq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3undkbpwt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dsuydrqc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3somyfnbc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbbwpgxm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eaixpqyl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3csnamlge.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ltjdvtwo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wuvhtvuo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jketypyt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dptnpmga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zgqlvtol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tthxuogp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ychaonkp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hglsonso.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xusvcerz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gfgwruxv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hcdzkisv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ulrbyqks.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ogmoaptl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvokwxr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yxxhuigj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wmrknmqe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3syaksyad.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ylavbdsc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ltfyjjxn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3konpdewi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wleoyxqa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kryncmse.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3drqllffr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qpasnxpo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zntudrmg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jwbziwha.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rhgjvrbn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjrlzqne.html


<!-- 参考信息 -->