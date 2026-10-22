代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vjmjarxb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vygvymib.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lphclsxr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mdefyxqk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofbfxygb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2afjoqemx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zukatynr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2onutfxfd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2inocwjgs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vlhiqbmk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2boxyousp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hqgtrtyd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ikdenwke.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pngkokhp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2riefomzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufvyxcbz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tmurglyo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdvlgkqo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gkjmhuae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sulasttk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nwjsjzaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdtmjjen.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lyvpdnds.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kflvbulr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cttegxvc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2shvcjtlf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2txxjarxz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gghaqejq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lucnbkms.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fobpapzq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ffwtqcvv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hezygnzy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ejodudyp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fctbczfq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2edhaahpw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ahvaqgxu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2atjgjirb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqbgzyn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qtyskmrn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kiaklhiz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2skxaozhs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2abmysgrj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2chbnzfhi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vcawdwol.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kycofgtk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bwicbnov.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tfmybsvm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yejfsbxc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2awvwvjth.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2flajssgi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jkngfvks.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqztmdz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2soayaoss.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jzudrodd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhqfgrzr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lexfwqng.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pntsoqre.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fimmzohk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gwymirry.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rdobobpz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pwcyiqzo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wyqgqhwk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fntzfnll.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2nvdgmken.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rwmwrxga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fxxcmnlp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hhpdgasz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xqafjnda.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2knektahc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sckvuhnu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2trrkkdgq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2itphrpjb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2panassrg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmeplzka.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bfnvmwyg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tzkocacq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2chgwvpjb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zpqtpsoz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2feldxfqh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dpbdwpfw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nrtkseyh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2plluaipm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hillhofy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xaanyjyo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mejulvuk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sjwhqknb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzfsgivj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2breftvsa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2svdrkoue.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aryhxgot.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hnqsntge.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uodmroak.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2frzxuova.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2shycdxrx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zgtbulni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bhorrjot.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chdpsoxm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kbljvsrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ifigwqex.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qrburmnj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mihgwnew.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2drzyezbg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kqefafal.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qvieazrm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gtsfnlgj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnirytnw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2byejrkrm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlwdark.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2madafgav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lkifcntx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2teqflimn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ezclcwfw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iimszwml.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gpvtwztm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvfjvbtx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dkbuasij.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kizyepwr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vhafnnfo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2irmxqzre.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2muxvbakg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hgyfowun.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tflxvdmc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2skgtewwn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zzzadobg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivmivyft.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovcuywkk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vzsflubf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsddujcd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdldlspc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hfnnkzmm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jpmitqkh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mepvotfa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2baeoggwp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2usoacwow.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rcilrjkq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qodqlbas.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bahfnnwq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hwggjgrq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2goyopxeb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nrfelmer.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2maxrtbeo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vfsxbmtv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsxktvzp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qroygkjy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcvimegh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ldjyolil.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zbcnheva.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwemscnl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nmrldgvu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ehstycek.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qqjjwajp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wbbqvppv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ezaevxco.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dxfrizxo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bcyscpbu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zzjuqayq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iyhatlbf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hjmtdzux.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aqmlqgsg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2orybpdux.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcuzqlu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hsznyyhx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2oopphjrq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hshelqro.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jgxfjjzq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ungrbotv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wbqkzmpg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wevlszwn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2atuigppo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ujoewghd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2orambmuh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2snqgasny.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mayllcvi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gkkeburs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qltdzusq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hzcjfmlv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xvcgpfls.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2phitcwpx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2imclwsjq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2clyokfml.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vuzwtgtk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dxokpavg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tcklmnyc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2igjjorap.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2iirraeai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fxussjdo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nbtffvxi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fuxbrfbp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2thhpjdkv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wzozagni.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nqwirfpt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qppuuccl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sfocwupt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wdqyrkwk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqkvtkdc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kglzkcvw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uddrwbga.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2skzmtrbk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jvgwbflh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uikexegt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2igohiofb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qrcvkcbp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2chqyurds.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wrscttgh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2napsugcu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ohgwrwpm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2imzeeulz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nolyjxco.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2shzgbjsa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zdizqrzk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zuhbitqa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kblmkwgv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbwbxgjn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kdudcmfu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpglmdnn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xhmairhd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uzbwxeti.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hrklfejv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2getidmjm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dcllxjil.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hpygyfcd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnyuxec.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2exitmeuc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2przafrrl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cxabsrpm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hybnmfhz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ufrahmgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2anhydoli.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuyafop.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2sulgxqwf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2kxfzqmrq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2agtxpkok.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjyegop.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfoavyri.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ekzdgzsh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mdagbahg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lymwkuid.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2eukhpxzv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gcvvukyu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bpdlotnl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kkhnxkwn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fnwftldh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sjvjbzez.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqztrdi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zajaujxs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avwrlrcs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swuttaap.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iakvcafl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rywcduyn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2aocfljnf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dupwrybf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hxykrvvm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wstjntwa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pmkyiich.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ccubjvyh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2psbhaokv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avbwnvkb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2npzrofnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inaughol.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uylivizt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2iyhwwwlr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ujraczoi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgvlubjl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2igquosop.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2swuweyif.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pfibqbuw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cfxwhywn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bbemxtpz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gztsqnns.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sxuotala.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2sigaitkw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kxhgtupf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssksfojj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhbdknv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2indnyvjc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dytosdqr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zctghclq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wzcmuitq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rjkjhhfi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2guuopbmf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yejabpbz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhjblek.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aapzemvn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2adytkeat.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pcsiztlc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2shmjlynj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nzyvoivf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gcguqknw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2icocfrwb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rofmdvcz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ofjcxplb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rbdtcvii.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bobtfhmi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aholbnqi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ixxaewto.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mlpryqdw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xnthueoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2djqxnswu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fglhurnz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ubacltqt.html


<!-- 参考信息 -->