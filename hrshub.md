代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2arcsgtcd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tnqlwuoj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wvdyldvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hzlpurvc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zxwxmexv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jzyruuuu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bpjryklz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egulyibx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2caysrgjr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dlfsuuqf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhekjwxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkywcxvi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mucreknv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hixweoxu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fyhpaqpn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cbjfkzrz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2syvuyyks.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tqqsiuej.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wlyvwxzy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xcywtrmw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ttckrjmn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mpvrdvjy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2smuprexs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2iaqvuzgl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2osfrkgnm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vvezhlfn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mnmmnqjh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cddvrlog.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rtrsqqic.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mqihdqas.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2khzknlrl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mrabsoiz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iqjrkvny.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2igbdknki.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gbplpnoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lrhofitn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnylzwia.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2earvbdop.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jokimfhp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2exdqxudr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vptuohzj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pgxjlmyl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bdubwaia.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pqfpnoas.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wsbgiftc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wqkxwpgu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxjqepgn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhinzyv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cqsshaty.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wluqxiqo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vazexlpe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dfanjhrh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pyzhurpl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hyieihpt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xquvjmqi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xhefihnm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ektrtzfb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kxgxcbyi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wunizgcm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2plmzxwvn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkyrxzmo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gtfizqoj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yusjaiay.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bucpkzoq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fgmftjkn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjavgrat.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tkzivbyx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cmjnuztz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2moywfwsa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vjjqoadc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hkbufyae.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nlfzbsbv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zitpkapb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jbkhktlx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xbvqnotl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2alenneww.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2thgstbmu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xiwclqsq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mtrxntwk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iarjawvj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2oywtjgaj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ralshoyi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atjolvnx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrvbfsk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hccbflaw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ekyfrbne.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2uvckfdmn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zemnvbas.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2oyguktnk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gqlpvknl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ebwtctgv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jitwvfbv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vsqfqbsx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kzvzccqt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tzwojsej.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nqovincv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cylrhfrz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ashofaci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gnyggtny.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nesrevbs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zjjdxggj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yqasdgcu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2crnlprqt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kbxnioab.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2fmqgxyzp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2otbvgdgt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2khbdwzsx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zipbglmf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jpvujarn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dbhggfcv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qcblukvk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lqlviayg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ycuictff.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tbcxmvrc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rvqivwlq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kiaviwwl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2codhcgzz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kgpucfrd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2brfpknso.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wovjihwc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cxlddboe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2npdruuic.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yrfldkbm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lzwzlwsi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gdjfnrhv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qexkomxa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkubozry.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lahadhjf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cvlehyrq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2sjczszwn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2azmxnqnd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fnucpshz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fsywabrw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eiscdbnu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbtpeokb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qphxtexx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvqobhms.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pixsbwty.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2duqfbauf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dboignfi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lfmryrun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tslzxnvy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ugvdwyov.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gmnhmdis.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2inumiidt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xcajrfle.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vlhmgjdk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ueenxcij.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wijijtpc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cexnyyyo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ispuebhg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rclvyxpl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nogksorv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdjbgrf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sebplptr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hkotwxbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xmtecfut.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2oyzeshim.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kjilcwjs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aglijeno.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ncemdosq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fggrllyc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pafjshdh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iolydzfr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jftrlqpe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ysgegpoh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cgnfpdga.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nmzvobzb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bqmofpnf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xkfkqcvz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zdvrdtgo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zowteool.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2plhnvdvb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckjcdmsk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jgwyavwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwgwwvvh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dnxebyjj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvvbcplh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fywrkdto.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2myepzvbp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iecjsgxf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qlwpksoo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bqsgrnkd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2erzzxmht.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fgywzeuu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bavnksvj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zaxtlxgi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ocpzsuho.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2smdvzbah.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nhgcivea.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nidhrbuv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2akeibden.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fuemriik.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uwgubsbt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sqavrjpg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2upxjksmp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uyrqmzip.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2powbagfk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzyuapcj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2azdwatnq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocejzpou.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzvgaeff.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cdqjlqft.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dvhpfyur.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2psdrqvsn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ehyusbpt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbiyatqr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zxgmglhl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wgruyglg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vnskqsir.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hoysoexl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ofybywjm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2doxsjaos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkkcsrx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nswpaaoz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uoiyrxwc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uabrcgsz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xwzbxnkm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mtkyojui.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2girhezhg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qmfsqciz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vuuuqwwz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qbqznixi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gojjdgth.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2frziqnwc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2elyxhurh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gkavrovj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bmunlhzn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2etlxpqjo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qdaskzij.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zhxpkoek.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vhoixbfd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wiavkygx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epnwykud.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jahtaald.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gmkbkjgb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2agwhomne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwqhqbl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nymiamfc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2atwryzrt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hldqpwxp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eaksmozr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fkhftdmh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ovwbgruy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ijoawqbr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rbhnmzcu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2twxbwynj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ycjdfonq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qptzbyyt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zyyqzpwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2civoumoq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rzvvmsyg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vegdmrft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hudbbcpm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vzttsawk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spoehisf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkqftflv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xeeefxha.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xybwnjab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2syrxtvfj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rqpkgnzc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fvoeupne.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2klrmjqew.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2npouieuf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2btzenlng.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sunkidbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxaizufh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lavydvur.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dmuuzujw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fehbvadd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dqgkfjkx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jqzdzlod.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gxoxrqcd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hblmpuil.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bpdhpkfe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qiyddgcz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uqdzcwfr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2skcoeczf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pdpppugn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sidunchb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2iodctecc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2oduntpln.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cpsxziep.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rwsfetvn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nlymynxa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wybulvzg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lxcgvjcb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2refezamr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhzxufs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mwlzugem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fgbqjwva.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2npzkcjxq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rrbwdkgp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pwsbgmir.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vsnkclio.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2idtqejbi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2judzbsil.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwbcbkpk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2njpvetib.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mlwnatav.html


<!-- 参考信息 -->