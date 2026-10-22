代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqhctljz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmmfdscf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nwkamter.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eauaowxg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hhpcboqb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jcmyzlql.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tswsymid.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2szcxunik.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nlrbkibr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2iozplvpb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ptrfifqn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ykmkeicw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kebfoagk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ibuvgjlf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mqajbccy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrjcvvws.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mvqvtswl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdibtfnl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tqixqmvw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dtibhois.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gfhqotqg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2asrmdqtc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cngshwcz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vwebmscq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ecgajuep.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2waswkpep.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hyxhnhkj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ajxpzhub.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zcduyjpd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kzfcqbhp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uhshmbvb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkxihyu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bpvqbwat.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wedbkjuo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2neauqpep.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yomrytiq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tqigyyup.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tuatabtm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2etxjjjua.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jahjoqij.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bvjdtdiq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wtmrssrq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kfveoeaq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lcaybxmr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ehtbguyc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxwbbgtx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xkymlbjk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjbuyfbl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mwvthszo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ivhszqmh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zmngfbbu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqvichg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ncvwwjck.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mqfoxlpc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hhxhyzuh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mmhfucbg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wzmspxpa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2acroaeea.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ghnsmhul.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xrrfzrjq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mrtjlzpg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2akxwgvyt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dqqgbzfl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jbbelchp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klyuythk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cafmbacl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ckhawjvy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2njnbirie.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vnlcsogf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdfaggou.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tefcdnlt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rmjvatvb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2aqaeinye.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wkcnhwqb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gkuxadbr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqvbmgag.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkgyhiqx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqvbbqhj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lpmgfpna.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eccgadza.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mugnghps.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ficqitqj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2azzrxgyn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ezwrmmlf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eejvcipc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aeybkvnu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2udqyobyw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pqczgajh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nunvvfea.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pvsrezco.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2edisshaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ydzhgexf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbhpncwk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cexkefsd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uclqegvi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2holrjrhe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fmasgych.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ukxmaosa.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bnmwgday.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mhfntbay.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rnhcqyzs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rioykpqg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zoaglzgb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tcswoojg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hxfvnxpp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hqqfjrrw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2swurqyjz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kewptgji.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ppryogpy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rmmayinm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jadfcitf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cveakmzg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uceogfvs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zupvqkco.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ikgrngmb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ezjqvqdb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uoixmjur.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hsacwdfd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ofmtewgf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fuiylimy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2awjmsrdw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wdmkgnqu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xmndxttm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcklddnm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snmsqgfo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dhsuasnv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rmnaladf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vwctbner.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2svvicaiw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqufmaz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ljbdxtmk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bozthjgb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ugdgbhmw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ucuwfcff.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xmoxmsam.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2oesvqfop.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2llilimtj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rkotxdtt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2frsxcbql.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwwlnydg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rohxtkva.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2klowebvv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cjquvlgs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iirqjfre.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sjzborod.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wmqhjaks.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhciydw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jafjwldb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wnbbfibe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2itwrhjyx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kcrjmpbd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vwdtlaty.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vedwuzsx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uscwuvhf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqsjbkbj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jccainti.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jpodbmnw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfavjjf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qnxhdkwz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vbcxizov.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2beiswgku.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ohfqczza.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2asdpcsjv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkaqsiav.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmhankhh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2adesdomj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlxtvxqs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lmmsuzdj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfttzjrh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dyaasfbv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gnbabfja.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ekwnqboo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sdytxeij.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mpiyngds.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ajgtiooy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nbtdyllp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctospntw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qcvgzksp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cewfeubx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkcfszea.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dbmytimn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jtbsugqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bkeeoxiq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2waymiifa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kmnbdvow.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tvbfmlhi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bmhxxqaw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xvlyadlb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2apozgxwb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2txlqnbov.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhyoork.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vibwyahq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kuwuqdvw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hhrzylbk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xqqlqapl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bhmdsntj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wzofqzhu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2krqcwrkv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2plxzlrfd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xdznyykb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bypansix.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ooojrocm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brbbtavy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2flfcydlj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgmxejoh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ayyhgtar.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rbhyxugs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rsnbtptn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmgeldqi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ydggsbxv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gphmguss.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2njjnswxx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nltvirin.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ngabsabc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2uzsepaij.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kvralroj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ydkcebho.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xhqvhils.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lpfrhufu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2joqunpca.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2aldmuras.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gobohqyo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kyemvtwy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pdvhwfhk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bwsynpba.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2aoonjcwr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wcaeffxw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2utepxrie.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vdflzszk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zyzbwane.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rfqzmvfz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2adycexuf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mkjrzmkb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ccfdqlmw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dmyvzzbr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ofxmmecl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bvwlkjns.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ktmcjwfs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vqtvtsoj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ghndzxow.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2flvrnnvr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pckavjjn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfbelutu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rolpkswe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nmhyitiu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtljmxf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hofvzife.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2woiddnzk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sluiohes.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2pdqkduaj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rbeuagpd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2winkhohq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlnijlfn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fazmzfmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdrpkskl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qosjnepc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gzszaopb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gjtjhypc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dfbeihbd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gicpxefy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lepjqkpv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qxvdcqjl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nqszumpy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kvxnzwas.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fzezcrog.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2igxmosjy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kkickdzd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gonodndl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uvamzmmr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eywqakqu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wamjccan.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oeecqzhz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2imjmrfjm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2whzudnko.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nbadtokj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hbhwhwbl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nlwtomrv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhptabnu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tdbguskg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hiupprgo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ddylcnjc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nwgpyclg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bguxbhyj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wnqexpsw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xuyejuds.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qoacskkg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mnspaqjw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bolyujqw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ckiaktvi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ezjrtecs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fsstpeic.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rafsreot.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vxyuyyid.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hemzjxdj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2asepjlsm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tnebuqym.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2trpvznpb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtvcvzs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xkunfpjh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qminlayl.html


<!-- 参考信息 -->