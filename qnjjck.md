代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cuamfnyl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iuuxenws.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zrzpndsp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nmszzthv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ntebbxlo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rozeiooi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qqkzvdri.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiqlcvvm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dumsmlnv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3inccazal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uhkrcncm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajarrtav.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xwsfzpln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxnpiiei.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ihlvpcgv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3moxdvyqa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wzvxtgqi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rgyqfhpn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qqiigbqj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gjjhykju.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3btmrldlc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ptrwyqhh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nivpptyq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vpjdnepo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3itfdcxeu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3npystobx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hnazgang.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgbfbdsv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ffybjxym.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hpxnpiai.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dwjfzcey.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eorgvsch.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ypdvkqnr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zduvgapf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fpaoegus.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3drskjwtq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ebeubulx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kxdfzlbf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3khfxtbor.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fkbcrlgi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3flddwapc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qypfxcvl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wzulmzbt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pslrgfhs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3enwmskup.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3coavaojf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3swxnvgpv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmyzdav.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tfdxxydx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lueberpu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dbfgjucy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zdjhqzoi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sayhyshv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xnmboxoo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xnywmayh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3eramxnuz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lgijyeqr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vurswakk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iyqaklsg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rksxlszs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qngvwrjy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bydnlykl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3psdkjerv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ytixjblf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mqwmffsw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bkfqxygp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3utgnpsmt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gxurnblt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gtucsmzq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3cmgfwgpb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fhdxbzmt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zmjwbkrx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptphdgit.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdidqwxa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jgavvjgy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ljhswjcc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lldagyto.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3abrbvwtt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zwyafsmb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aawwjjsk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ubjcprzc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bpyjtqws.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3anqxbupj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qalgpgda.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqgmuio.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dqattbpp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xrwvzjym.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lovbbobj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebcsxdpv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vhsatsal.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nlozxxlk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vfxotvlz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zfxcwoor.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nynxjhlh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xtoultku.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nodlariv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwoqbfo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3taghzhhw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mubafllt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3whqlpcpo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gwavomib.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qtxqrtmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zbsrjepp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rugbxunx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hnspwvcm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lxtgnluf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dzdagluw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rhzrojxa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eaaxxbgc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3swwjbcjb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkszsmbi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rgjkbmcz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dkqbkibc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jfljlsas.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cubyvvlw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kskemamq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uducfbln.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bphmvtfp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vdgxiqhu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzjcoilm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rpinayov.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3oiojmmep.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vewsiwsu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hzqklyet.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lsktzxys.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rwenrokd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3odaxpgcd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aprxtfys.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tnxymabr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tqzxhagj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rttftbex.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vjnmrezk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rflcileq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3boiravvs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyywcsag.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kokxblus.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ejfhnmve.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbsvwmbv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dkvmbylg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yjrcjlvo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3magxfxjz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uhjseipd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ljckmsya.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vsnxzjed.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3deewtmql.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3sfqwtxbi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3orzxvezf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ozmofqyf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3thlkpusc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fvzfsrbv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwkvmrxz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ogcdutnk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lsaxzejw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ltfhgvlw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qywcyptq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ijxdmwkj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cjscsztm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dvehcptf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dsahzbbi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pbyykbhd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mimumkpv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dvvdtbcy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcqdrvad.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rcykasif.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wemuppnl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rnmttmle.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lgoxwnsg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qxjtqjsp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cflcosyd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qvykfpfd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3suljbiic.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dumvbowl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mguvtljt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wskwgmen.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3baoglkmh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkuxmxwb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3txkzkufu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3optulhdn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uiurqsme.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fqkwxvbk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vswsfewn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dtniespw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rweryoxm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3knmhaabj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jpbrukrj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wpfvmshb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yownqesd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wljahhqo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zldjkomg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wulvwsvh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3piktgrzq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ohmavvxp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3owacuihq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ytkpxvjd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ongaxumw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ygqbellx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jnrfadag.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xeauasvr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tnulogtq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dsxywyrf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfkzdky.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gafuqgck.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3znjvjdiy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ksoncxku.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3smwzvlab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nymgqwgn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3abdfnwal.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wwhuilgy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cpnkqzzi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tjyjpgij.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sonuzcvf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dlpkxjgi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sykkjxvq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oevohndh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqnthecg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nrgydeim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmrtkxi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qaydzjst.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqzfwwru.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jjuxkqia.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dowewtqs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vvohjowj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3miujkdwv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ewxyllue.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3spbhgsrp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mzpixxwg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rvbkpkgy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dumwiqfd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wkmqsvgy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iktnbali.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rrkoxvdm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3svvtfqsw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ldwszlcj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sorzsejv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3adoshadp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3klbznwfd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3feazuqsf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yksffmei.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zicllzul.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zhwvrolz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yuburkpi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmwrijh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdlysri.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zmzrryut.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pspgjflr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kgtlwcbh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3knxmifuj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ochxjplq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axmevzku.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ncuqmksa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sycuzhtx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfosehss.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cpjgjrrw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3buanljko.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wbjdvivc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qppcqhho.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wevrdnne.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3undlzgzn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pzxlijxu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xjujlnig.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kozyetov.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zytiyhpb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3olfpgdkp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwiquzj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bhxfkytu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xstljszc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lfztbtgg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rgtltftn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hzmoludf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sonvctlt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uucxyrqg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ksiwrimq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3trksjlyt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yzumhedc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jtsbekaz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3onhdlqmd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cvsruoap.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3esheovtn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tvizhblu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mluewepp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gglorwwv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nbkxetqk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rqphjxrx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3forbecds.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vwvtxwdb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvxwome.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbbyetl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3okdfmnmk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hedvhqdo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3habehjbo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rxrqknbb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mszfmztr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jfgazljn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kavevrba.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3idvvfswr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3whqbwmdi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3obmjavoz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvkhmol.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mhtlpoip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ixubrrus.html


<!-- 参考信息 -->