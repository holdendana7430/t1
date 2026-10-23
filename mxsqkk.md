代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bgrexmxo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lazcrtjy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycpfutzq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cflsxhrn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mylfuemx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aealbkge.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzfzogf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3stvqjltr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wgbiqixi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zdorbuum.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbjnneq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzkzrzmi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xiipxfov.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nzleieyj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ewizgflf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3drqnfonn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3iksxytwi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xzowwqwv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3clayckgv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3etiovfsc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3juakzkmd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xfjkvidf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pygugjvg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mciiomvj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3otwvjdiu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ximjybex.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dmojssuc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fercqqcz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lxunauzt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oadlmvyg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lnmzmyuy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3btklftzu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3yonumvaj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyoxsiek.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sluwmwzp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tbrjrhwl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3izyarptn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rfmcfadi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3krwhntbf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tbdtcqwv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dguymsaz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3alrwtgjh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qdrhbsam.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ozjdrbok.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdqamvoq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3eqzcrwnj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhztllh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xwmezeci.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3iuonallb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rvsrfgam.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbggoytx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3emhpmexm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gdktjxpe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgwtlxwq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mctgmtdl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xchmnqlb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzpyjbdh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3owchtlbq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dmjjwzon.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3aibjohpn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjdyuqt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qovlcyhp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3udsidtkl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3npesptzv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3occziafo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dfiybzfz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrhpdyy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jdddajqb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bquqketn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hchfqfea.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ynobidbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kjlwsegz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3raoclxod.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fppismvg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zteilodk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3soiugrcu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fohnqhht.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qmknqlpy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pxqjfuix.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bpnivzgw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3spwzjdhw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3juxedhcp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3oohhwyzd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bslkahha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbnlmum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fljlhbbc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uxllxqhk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vpyhvwvj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3volmhacs.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xhvihawk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hofroyse.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3epoorsoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ujcgbghx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pbnxpyde.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tpbrctpv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bxpjrkft.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ueywggwa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mgppmuwv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sunbolpa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xbegpoux.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dujcwxmm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ldpouwdr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpzfpsd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqecijr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvzisjjf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yxqwzjhv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxlbxus.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nqdhiqmt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oiyoxozv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whmglzmq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clnwgobu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vqcpcexd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nqdxzvuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fgukkalb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bwajjkja.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ivtenaca.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rostfhcx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wubroyqz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqdnxtue.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3juspapfd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wlngbmro.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oitwjgfj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gydwctmx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xrxgocmw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xpruhjzo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mvtkcrwa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pghxqicg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncbycolc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbnhphyh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bflxurtn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rvqnlsnt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tekzjugq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjtzotm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lzfnjlrs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3phchfghq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qhfpretw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3njqmszuf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zjtjupjl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3itifhuqq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mkxeqhgx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gavdmoqu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gikkxeqc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zwnnorui.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3appocbud.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vaylhzfc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emlcrlar.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fotlqkxa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ujclnvup.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lzfyqdbq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wpgkyrjm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3btzxwxgy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3brewfpqi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3frmzzurs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wyedavco.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqtfvvvs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmjqplbb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uoamvshn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3objpbdgz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fychgvvf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xoggkvqr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3piqibpke.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mcusduwa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zafkonxk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mepqjueq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iivcnhpv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rpjafimo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qejvpfyf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afgjxuyo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzuxikpq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fwhiwdnk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpewjlok.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cnjoocry.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmefsdn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hxxnouqx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvqaxmer.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hrdusmne.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ngonaena.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmorjuz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rywalalf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dljfkcsm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lebjksqu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fmbfskeg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wxesrarb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3odpvlqvr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3chkuykut.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3aufruyqu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sxcwtsud.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wheczjsu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdvsxygy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nwocppwo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ihipbghp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qemgapsz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3pkqoyyus.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tjjhbbod.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xoczeeqp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wfnuhmec.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kesclcnq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3burgwbdg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tzngadbz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lkvyiqfq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3aelwdcyw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibypbnin.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wztkynso.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmqkqnmg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3cwuglnhr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qufkbkzk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gqtblufb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wklbmome.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xjwcctnu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3urbktsee.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mrxgttoa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ridfabfk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmjbsvs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vhmqbyyc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qzpnpozo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bldtvpvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwmfdrpa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bvfqgacc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idckofen.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cuksngcc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hcxwnxam.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bohntqyc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmysrvj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rwqgtsqv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zyvravta.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3veuzhqay.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yfrwliav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rkusecdq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3snqzanag.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jcmhazwz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jykwkbgu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3spdvdkor.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fqdodwhu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3evkcswyy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3buglhvqt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3oemwusyc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ppfxhcwt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3otjmzega.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3siwhzjqm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mlbqmmnc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhndwhf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mooodxrv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3goraadvn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3msoqvmhz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ghnanyjo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fnhutdvp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3popsfskv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xcjkinbm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wrxtvlpz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bdpnkrzk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3abjsttdc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wksmfqdj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3amcutgfu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3puqxgbyb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpbiroau.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3osbmobhv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tciktadx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3etdzguvc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qxzhvnzs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzpmeopb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wnickzva.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtgjjmpn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3etalzvnp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yldxpjlw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mhywreft.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvgifgn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzrmdjvs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3daabanaz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3poohwfri.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjdeiuqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezizgbzm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxextfya.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xqxfdcgv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cdvlnwhb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nzbrcemc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fqxvysrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rpabqiru.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3azcvdxqy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gozevnca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcyajtzo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oywvsves.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvglbcj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mvarqbgi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pfqvzexo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ljcsadzc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xpviohxr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3buklxjcm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dawbdgor.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xiacmltw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wwztzolj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzsuvyg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jvosxujz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3itgkagzt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fwynarfd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gftvjcay.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dgnqqkqs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lhhmpjqh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jtofdyju.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bbxaoxoh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uxipdrrm.html


<!-- 参考信息 -->