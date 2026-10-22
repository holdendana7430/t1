代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nalwtuju.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hrxipnzh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ageyjfct.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rbqzhgvv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iojnaafj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2schwbvqh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hkxmyuay.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gnqcvzme.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzkzcbmd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pxknydmn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kxucxwyr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qocrwwkq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wezxazly.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vqrtmqvf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwusxtan.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2iehzikqx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2anrydukq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mhzgayun.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cchfhgxk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2smbonxmv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2flmwcesq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uhiyakgk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2elqxozks.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lrxtzpzi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cawvryuh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2shohwtro.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xqhtbbys.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2scqbjeis.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ayuuvjzl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2stuxsvjx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2depvsiqs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ioouuwlr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ljlxtwmg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lthefdwe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rpjtbdvv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2oggwgmzp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2scemjlpn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gtlepjue.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fpfujtlo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tlmxearf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjykhdno.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jsiuulcy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kirsimfv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bqbjaizy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cwdqscvg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2azqybxjv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2svpuwwqg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vvghpmst.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nqwydcwi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2unguzlwp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jaeaglaw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfkhyedn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kkfktxcq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mggpzlox.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bfhyfqmr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2krqujvak.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utlhyaka.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2axlrroeo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ygxygcsk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tqjzliny.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2glyiahhy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pidqnisb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mvooicis.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nfmoozhp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zoohcneb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnlaorij.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ndpsummv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2puhccnue.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juidlnrs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2owdxwkyn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2yiremnnm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ixerfubh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2toibbhsf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qzkhfqyb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vmbydqef.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2orhjhtkz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iicoqeiw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2owtdrdmd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2txbstxvr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2btweiwij.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qvxqhgzw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bhplmfyn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hhqdbcym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fxcuycgr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gwvynqse.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vwlvyaqn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtgouxji.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2plsrcbrf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qvonkwfr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2snliegzs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hwawjqje.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2sciltixf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fbauslij.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ouafqzqy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mzgxdzlz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rrpkmfsf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2edtgfslt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnkemiw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2isaivzum.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tjqtaytb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2upekfeni.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rvllxvgy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ygipazuh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ocalzjpy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bmrvsrtx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dfjknskq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rodwhupf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bpkvajet.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vauvjble.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2icaevteo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rejiikvt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pllzqavy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dvnxhxrc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmqejgdu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2negrjtex.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2shvhpfob.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzgpgnfs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qqgrnfco.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wabziiij.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nonkquzg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hjddfogz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iwhzgmae.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vebtzcxl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ftnkefub.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2agywevoy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2oekwmytk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kgwpllce.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zwzaouhw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eijqnnqg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rsepjtgk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2olmfjben.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hkhjnpzh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dxushtxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxobbth.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2agjndaqr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2txmpexqp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xwrnahjf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zryiuoxw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pirobleu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrazvpl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujwdcccb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2woprbdwp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dlnuydli.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2asifcrkw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owhtltko.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pksxpiwg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2scfgrobt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bryqgwtt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wcspggop.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nzhnsgzf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zivazgdu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2frtdnsry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zoofejmb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zahppsxq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rimjplsf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aapclljo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xcqlelny.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ffshetpi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2irjszkkk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cbnlqwyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kqpfiscs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2mkwmdgiu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fevikehe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mdrxcysn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jsejxxkq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ldhstxjd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2krkylkdy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fupmxfnv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2telqrhbo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nvgzgnwf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vgbynuiz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nyllejff.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dosrwvhw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2unrlfnep.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gfblxmoh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ewthigci.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2stnlvlcs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ecizhwoc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tkdcehll.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xifiplnk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsnsojcj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kryeyjbl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjiuiamh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mudjfktd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ihfewkgd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xwxfrnzx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhqwerb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jrcyqbqa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sbfelvhl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yorqbwea.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qaxglsju.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bkrqhyyl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zxlvagga.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbsnizs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ufaqvwot.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hzrugpuz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rbjypbjh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nlntorrw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lvvfokdc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rebkpnek.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2imrdiayz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2txlmczaf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2skkbjqnt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dsdumgvv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zkzgallp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kugzphew.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vntpjbdg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2eeaanwmh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tdwqnxcg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bjuzgxuk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2sivggkhp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bvxzvbha.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2maeqslly.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rscaajpz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xshjpczd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pqanfrou.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2comksdqe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ghhfotmu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onqcezky.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhgmkrga.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vwhcglwq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhpexayw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fxllducs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2keelssfk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2efpirhwu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2affnsyus.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jzjlrlqs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qlbhpxmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhtqqhzg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xmyrbzec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fznhoqhz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2plzduiwb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ivtnvjkc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xjdbztkl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xsodidiz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eidjqzxc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjkbwyhj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qcbdtupx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2czduiyql.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zvltrynd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2caekhtaq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rwjqnelf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vuqjlhhg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqstfak.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2matjkcia.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qmzjttcx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2acninevw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lvgzpubm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ufnwppbk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ktwbigzu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ruwevnbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sejtyeiq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uirokmjs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2szadqcaz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vdwktzwo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lsrtprys.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkmdalvc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2goifawfk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wwnejqci.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2abqqzdxj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ujcmoecw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qkulumzv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iantsmoa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2erxrjagd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hiwyvmiu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wqwonnzu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xhtyspyz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2neelzrzt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ssdyuhcb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2okzusdxm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2innfsqxk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mfkntkwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jqblcxaw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ecysonsr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2amtuquze.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ziwovakb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gwzyjixg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2unizfocq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebzvowxj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2flahosun.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2glototrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2upzatree.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwumzpqo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2orgqsowr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2piutqftv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ifiylqjs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sjshzklw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ndnayyvb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptaayrsm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2israwpic.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tbzspsvy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzmmrkj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hyibmnks.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2igftvyqv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2perpeuzi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bswztfky.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2txoyzytb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nowwqddi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ikphuwoz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qmkxwgym.html


<!-- 参考信息 -->