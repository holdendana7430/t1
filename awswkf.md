代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jxxerwpr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ajjnqket.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wbukrcoc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2boleoerv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hthkjbts.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ombwdclo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2eoxwjuiz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvfjmzsu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pkizxqlh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zflbgvam.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhretzqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgkehlgk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2uxsyuuwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygvnppmb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rhxcjotm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sdemoghp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mxefqwjj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hzkrgkfi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gwgesmzq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gecyhorc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cfrqtmpk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxruhm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sohbiske.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ltagitss.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2htbrfpbe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qezcqige.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omxelamz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dghkktzv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2karbbwkd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2omjctnii.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ehijrxcj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nbdtnbva.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nmbjwdmn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2shtjdbms.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2isdtxmmb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ovpcdhpb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rtpasdtb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vdabcikn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nzsqmues.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2chhokwzz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tfictszx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wyxrratv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqzqjkrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mywdpzfb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2istrwwuf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hrgodjbv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2knqhtput.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lmgnktvg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xibhjaqi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qexfmdgd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvvnslhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eafoeshu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2phnmevaa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2caokompz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cybkzntt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jqewwmnz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jodbmfov.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tphmdyej.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qwlbaqwy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mirycqka.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqcznjbq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hneyrfbc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vhspqvhs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pjhqctiq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2sgeflnma.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrepgqh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hkjfikmd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tjdptaoh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dbhtzofg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gniozwds.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nccgpdit.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ftmojcnt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tcwtvlji.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sultmcls.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2dbqfbppt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cxeacxcw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dmdgttaj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cnwqweew.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2liffemfy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bitmsbnq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iabytzft.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rhdzgxes.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kjcarvcc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yctadmoc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ryqzcexl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ysrrrrsd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rnaookki.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2osvspavb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouzdyyza.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tjfsomdn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ilrcceei.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qbbjspbq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdzchthk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2apyzrzim.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fqwkgjll.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bhfrmsng.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2glprkaul.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kpzpqhzz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tzmzbfjj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2clwuyygd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qhmndgax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wdofqyga.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2varkkpij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2juwcopvv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bmuzfuag.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tkvvmhlz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdvuzmzu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pilsinap.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vvgcmdgn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jsafvnoo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjykslkv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vlxrvyhh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nhlurmpp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vpwobvpz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wpesgkxi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uagrektw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aiymnmpf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmgbuen.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nnpyohis.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qtgsoork.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nutfmdja.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2oxgflqzv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hbzizaxt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xhmhxfvv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jobxspbn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2buiblful.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wupnagzk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gkvtwouv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fchqzezb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqnuxvw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2voyjfgam.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rijklcyg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bcvuxsii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jltbzywa.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lqopxtnf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gkudmzvq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwhffnsm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2upjhbjsa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjcgfom.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iizovynm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2anjbffuz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2urhrnftn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nqkzftya.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2etxwhfis.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qiwxfyrr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lwebhzur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2eceupnug.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tbaulimt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fjpfbkel.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rngqtiht.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwlhbzjl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dkrygfve.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2basoznso.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrejstax.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uvxlptza.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mdhshaxw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dhlpbldx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2foirzhwy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2unximaxr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2loohctya.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2piebqwco.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdyvrgd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yibhqrfz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jczjpvqb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pwoitosk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nwwojimi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lertnjhw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bvdsgiyv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qvfskrxh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wihntfgj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2geczhevd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gfvspkln.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nwtcfery.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2npafqpnl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2aszrgsml.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lsfaljcp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qttgoeer.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kperyayi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yehmkhgb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bcrqetja.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2czismbrl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kllyrskt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zjuruiuq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sqjzaolx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kommeuwe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2eueqrhbd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mieyshxb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ixymcvvo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zoebyisb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bpswtllj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rubwcmuy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2glplhmbq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ccnfwtdv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqpatf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dvkwaeop.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jfddxmtb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2akzuqqol.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzdaapb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kfaxxnvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvkoqtd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bnnozcta.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgvnffqu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqevydp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ykxcolgq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2skxakyxi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jpayrfpl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvheygso.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xfuxgsxk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lxvnyyga.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2aminyesi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2avuxihfm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mpiwgbke.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jeknqpai.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mokksmad.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2klkfboha.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cmidsxiu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wxpmundk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2miuwcqet.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnqlcgzk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jecfkynd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2apqfcfcr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wafeqtex.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxfrjuad.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wlkssnhg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jhzpglts.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqayvgbm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzwmwrpl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ppzdwjns.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sxukqguo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bdgwjotc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kgofmxka.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2znewsxua.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2djetjyun.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2quriojju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzyobwws.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocmwfhuw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bjsbtxrw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivertymn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lxzpsohv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oqkbhewj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fvvpombv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmcakgaa.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xnrbbivv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bkuvfqlk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dhuzurtl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2drhwgnjy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2knvnezsz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uxynxwea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keubwdjw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xqiavdop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fogrpats.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mtoeenrf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ptqbniyv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fhlnvghf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zktwdqow.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gurhthxw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gewatyer.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ehjpjnxe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cxsuyoxy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vchgcszl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ingnnryg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2acxpoble.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uvofaojm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2whqxlonq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mwwkasfn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pzrpqqhl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mvpiwdye.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gwqjvheo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2axvymuhq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ysknstwx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fmwufuwm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dmpstvck.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bjrhmsph.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2btlivsdg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vbbiezwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fmsyalvy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gfybzgxm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsdpsql.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2betbyyxv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ospdcwwb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mrjudirk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2omxqbpzz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ahcokqqt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zyjfcogs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2snfolbxg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mmhyokxl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vprllokc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zmzorzdx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wdxiiywz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hvharsxd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2djbzpjzh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjuyrif.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sfxckkkw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzzcbpax.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tbyzxxcl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iajalfbo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jqfyflow.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlkdecob.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bnjsmxpf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smpnreif.html


<!-- 参考信息 -->