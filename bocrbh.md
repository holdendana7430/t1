代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cltvyufk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbhmmnos.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kiaprvdq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2pwhcoyul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2frzqtjyj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bxxlfznb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cadnfpwa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ggjcqbjl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cfxiytzl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mhdphtam.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ookkbzrn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2cwvlijkw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hdjmnpnp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ttfmldqs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2odanmhqy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vkqpptvl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oxvbsrnc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wegdkhil.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ustxwdet.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltiovmjn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dygvyyuy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2haqnwudy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbwjrprd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lbzbhezr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gurkqfof.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oeiwvlfc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hniuroxo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wdswsayl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mwggjmyo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2azjbyqcr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2beapyrdf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rnzeftlb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cdbsncos.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wlcqkrhz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2boxtkcvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2btovtzar.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rpknjjei.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2aroicfxx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jekubdvq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jybemmve.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yjxpmqvq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2erqexfzo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2siottaib.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ppbjahvm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2erjovwiy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zgbuamls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sfdvwtrf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2swntlxdk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jodrmlzr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bdyxczeg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sdoxaxwv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cfwapyih.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kwjlpxze.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcmkdld.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gtxwpowo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ifguwmiw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uvhosrpi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wczeushj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qcfswqjn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfapnmby.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2siinpvpj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fauwzlsl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2uzikxpdr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yejlmthr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jvipafoh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yqiuhgia.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jbqmspub.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2afmiqyjq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qletwpzj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hmdilehq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ryxolvzy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ezcgspnn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zadlhdfv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hslppclc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2folxmjnk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uikcqigw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmiggrbt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zxbfstlz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lwanmqwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dawfqots.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bntcddha.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2htyqyicx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2yuesshjt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rxqvgrcz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fbydlzuh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2evigedkn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hualmlln.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cgdumals.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ndtxmpai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kebsildn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dmnwmdrh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kqvvkfot.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jhbeezwj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lpfamzxe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2szdhbkhu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dbgwdotk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gsixyuij.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dmmjqyey.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrxotvx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2obtjooak.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2chxuwqbg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qootcqbp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vxkkjjby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lvbdqcva.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bomyihgr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yrhamnwz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zsdjanvf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pzxltpxe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrylpgkd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xjhtmyqi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hoyjkfjv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dghbhmry.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bkxlwllp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwtbtcy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ohosmtqs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2meyqcswn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ylwtjebd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cfsrxtuy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qmiscwkm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yvwtsywt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fbnpagyh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmhoacau.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zbgoymbs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2blobsdwp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sewslwci.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2btaacsum.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfnqyltu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2stagihvq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ygspwbne.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pvdjzmob.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngldnfhw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bsnccoam.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nntxdkno.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qrpiwsdb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ggmvrmwv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vmjvmjkx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvbytsv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ipbyeptr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkmlnbfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ayisfzbf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rqrreven.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ffloudcg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jqxrrbup.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uaqveqcq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cwiwwuto.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2afkncbhy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2akinrrks.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmjxtwu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rkfqnkil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ilnthzvv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xujmvttw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hqdzrzzq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yiantjfp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sacsboez.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zumqmcrv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2btrzepqc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2eywokmvn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fowxtgil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ycvmacoj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tsbyjrnc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2likeaftc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fxfcmbqu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mcxonsdv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfhpjboj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ndjwzbno.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2elxnqyty.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wwjngstj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aqgvblwy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xcwmbwkd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qjktdedf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ggcdpyyf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zbxpjlzc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xwrxings.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2aglmeyug.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spebzplq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hoiajqtg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bycfedvp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ijaksjlp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jnnznbhv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2eamxtibg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lpehqmdi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2aojhgzyx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ooukoilq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fbnmnlxr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uznyjxfb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ijsgfzzq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aygfatvt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imuxcytr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2djgfqgei.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oxsijyia.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2auvkalwm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yybepigf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpbiuqsy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dsgunwar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrpiepqd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jzmuhxli.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fglvexto.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fapxcpsj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ahlsmvav.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2psviuyrq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gnkquisa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2whkrroso.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tabtlywg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kfrhspdg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mwlmrvlj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mykucfrc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ukkkpxse.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mwotaabr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgitkxso.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yvdydwxf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jcxjzyut.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rgznoaax.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cfvhrbur.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2baxkibab.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hdeoujji.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ltmdrcmd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gazeckcl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2axnuexaq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2okxnrhfq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2evculowo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2otbgewzb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdautiqw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2kcdiqxuo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lnynqdvz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yslhxpzy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hmhnqhgo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odbwrkqb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2udbrbzow.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dthocyfy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmsclxev.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2thdgexyi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zvoqvyam.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdyhmgd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yjagcqcr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uzifbxuw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ylcxcmku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubkcrbfw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xzndcniz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rskvseyz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chptbknx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ublwmvqu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lkdrdmcl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hbdftgfw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2erkxitgv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nrvvpqmc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dnivruaq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zwwqdttb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vbopnybj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2papofowt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2byznissp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zucaqsyd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbuejpi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vijpephr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zugznujp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2sirnkuxp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tlgtcyxz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zpeduwvi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ghvttbez.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pbpdqiva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vvscvege.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gcscevod.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zebhndrs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vqwvxcoe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ipxxkhls.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qrbufaff.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dxzthttl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ffrqkign.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tmhjkgtj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ixccukpx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqpbhhw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ekecelfj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fltqqgwe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2csvphagp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fvijyhgv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2evrjmjzc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kqzhsktp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bthtxfpi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fnowweks.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yrhvubeb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fwtiivrh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pxmhqjkm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fkvpvrnr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2uqjecogv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rhbpfqdc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vklylfwq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2chpepkys.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jkeompph.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vduwuuhd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bjwhblvj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2broubrwz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aovanusm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fjcmxrfn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vsweueeh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2npqfoydj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pyjrvcws.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qfmbycoy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kllfjkvz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fscqxgct.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ykiljyfh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obausigy.html


<!-- 参考信息 -->