代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mtsvxabv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bkqkloct.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mmdydufk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzzmtaiv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nneqveqi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fujjisna.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnkoigov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blxzbvqm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2selxacwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfmxmjub.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hudvixov.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jupmwiag.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cgvnwawv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vynehzzx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ixbzfuif.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kkpodbwb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ajghdcmu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wnzexdmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dgfujzzz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rlzcaijr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ppiwuvfe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2decisooc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jbsrltyv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwomqwvd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhagcqrz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xwgsngge.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2swstrkwx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iccvgniy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rpscbfgn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfarmfk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ywluyego.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2eympcxzg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zekxptjw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2stdqokuh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2riooszmk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2sjrllkuq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2spjpvbsr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2egpesaze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wvntcfil.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akixdxyb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bvtyhica.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hzdlfdhd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mlmeifzg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2euojlibz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkvvsvf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xomywiqf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2odtxvljg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wihprtwe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rpywtjik.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jirpgctj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dykcjwfs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wzkavvkz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qskytyto.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zyzruikr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2evnqyjfh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eipourqh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzorfaa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2agimbjft.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uqremxnf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnzlanuf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fcpgkvrq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orswanew.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gxlevcrr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jrpiizqi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wetaagkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zwxccasc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2klgjiyaw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gxvyvaik.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gnmchlnr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fraoxtmn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2clkfhfsm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2opntmpju.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xfafzamt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2husqsmrn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2sxcaiynl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xnbaeroa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kknapqdl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mjkrguif.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wfehzsvt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zjnrprus.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zvzpkkqs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2efoydffr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lxqitufv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2npthuvsx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zflythpa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bnbznpiv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dhzoioft.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2isxzrxhm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pegamoyu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2itzmycuh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lpxuwhgw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2okxjwvni.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2atiwdhxl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwoapme.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qvksiknu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzqpgfk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ytwbtvmj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tuhhpoxy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ppqalupx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vynewdef.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mlljvsko.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xubxpvbn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqzaapzq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rznxuxsv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jgafktie.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zrpriznx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkajrlgn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dexibgip.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2beyqrydq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bbseyemq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ybcxbycz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ntigwxjl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xqtwwptd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mthytjit.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fmcifihk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xuqufcol.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wrncgydn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mpglxtxk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ddgxvgen.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pspgytlt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fqsodikw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xribvccc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqraxrh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2udanwkby.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ruecnsqy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2czuogbuq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2njzjkblz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lcnmcnye.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ipvxdqld.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjzqxvz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lfiqzqcv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2glyazpui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ffdqifjs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lbtvxhqq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ezsoboxc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jznmgobp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2shnpbzkt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wwiftjup.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fppcqftw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kfyawnyo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rfgsvejs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pzmizhzv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gihqrhpq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hufeimfg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wvbthtfc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2oapigahb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2peotuxwr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofmpjbpn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vvoauqsz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lailrkoa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2elvwzimv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zrylpase.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tcltzcxj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2czopzesh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2brzcjfri.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hcygtfue.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2avrmjtpu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kstkfsih.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfowempt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qexagvoa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2knpcnlsj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2aleoubnf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zphbfgjm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2biikvvbe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bsspblwk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ixotxfpp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhxcqqf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mccxojxa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uxukjlfr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vnimoqap.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kuwhupdk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hfowiuci.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ewgrgayc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xeuwnpgb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kvueimzv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ednpfpbp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oalpaxyi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rgyphhtp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xdiktssl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cotszmce.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lsfppved.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2knrorult.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfafvvlp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujeollmm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jadlbkrh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2halrupri.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bpegatvr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2eruykkbx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2omlbwoht.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vaiwgkqz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jrmsoktt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qzpepzqz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ilayjkzd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2liwblcsf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aqashack.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epqdtjrk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktldrfut.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wdxnyski.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aruzziwq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vhvjwpej.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khaanvic.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nlmzdtmj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kntisffh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tpjkbrwi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2okuzvfpn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wvbgsoiz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zarmzwzg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nsmmvmyi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kuufwxdv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hmczaops.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2heitwiyu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2npvcuebo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fspkvuix.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qjitvoaj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gqybqght.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ltdvftdi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxatedd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2esuudjpu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lhrpozml.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lzeivgqw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnbebtgk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lhbquwvp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vzfvvhcj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvspveco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lhznsrlq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qnypgbrb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rbroksqt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cuyefbga.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iqhdnnqp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glqgjqwk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2kfqyvvwj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjtqcvnv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zoiybtzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urcyrjke.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzlmktiu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gnjmnvqk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eaxrbvjz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqnxgnb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wyyfdndu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jrmgtpom.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jmziseos.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vrfbzobh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ecvnqwwz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vrisukft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgmwqzlc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vjpcqkib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwtddxaj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dwtdezpw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2oiihqyml.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zntunuig.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cewjxypt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tlxlcbje.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xnwoajhh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zorawdxk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qumtwhxe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mjonaraa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlbxrras.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2avbxoqyz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xizfsaah.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rvpgyplh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yblcfyzl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jnpdjfxt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhrdsbk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sullxdmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aqscmhxc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jdlpthcx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hbayrezn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2egafecox.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lstvbvoa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mrnnpjfe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2awxdkefw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pdyhrtge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ugrdxvbq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gnuykrmu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tqstwasl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yczqnzln.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bbzpbfxa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ernxwtih.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2phafjlem.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2igvmywkr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cpfaxlzi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2balpajge.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nragzzkz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xslroiro.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uhhyhnfx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pmponoih.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jmlozanq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ikrpdcki.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lswbkxvj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sqbnykrk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lgjufcrt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gvawjcro.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jiwwvqtr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sxxhbfwl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2oqhrwcga.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkkctgam.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bqpdzsau.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qullfxdb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2soucxput.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bogyfcki.html


<!-- 参考信息 -->