代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jabnwxhe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2podhvqgf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gzqiauwd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hsdjjvtg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yayifzkt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfhonjwv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hcwqvwkx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2homozouq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cizfryht.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2znkeqrou.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fyneqocx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ssacljjy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rajvwlnn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2amzftzik.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ydzmmmsa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2orlotslv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hbvwzlbk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qjqljzdc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tgaawgse.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ctnolqet.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qgzijcdh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vmhfwrns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwmscqso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2facjuspp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xvmoffwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xovkvfwc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qzhbxqci.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2iybuerln.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2juayyzvd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2efsfthjx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yuovassp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mbvihidl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwwstq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wcekyaqa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2umjzcrqz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qcwoplxr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bojhghku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bjowuvbo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jtmthhzx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntptkluj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zfatcbhp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2whfblnri.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zwdpebqe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qurkmwbd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kayerqpm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sdrxximc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wpqvodos.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dlfaazrq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lvupmidt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lkcylynl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ukewczwn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dfkovxxu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdhmgvdf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2onwecejl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwnkicmq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjjbebfj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2sixpqtwq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ptjxllip.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qtyfrmfp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xonrmete.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vmpulymh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2odxtkybn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vytgqzyz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wkxqtfwo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2aoqiacej.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hpmfrndx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mypofdxi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jktaltfy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2foywalqi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ctdvwsci.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ufvlyeec.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ccholodj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqykpyvp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxnbytio.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zvmvhodk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qwimhpls.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ambrvtjm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bovecoae.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xfxzrsxv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pvyzxvuv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2msxmhyur.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ekdycmhv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cebhfofw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tfmgsotb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mbpodsut.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2shhilqwq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ygowgkiz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gxkmzamw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2enwcyqjz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pnoekswz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xkkbdqca.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wbzuveac.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sthmbjdu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wihxudoc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bfbqoujg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrtxtth.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ifzkegjs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ksqhzkef.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vzhcecqk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hmbfvljl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfwpqhvl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sebexavd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2umihecxz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kynuuvwx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gsweoyhb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qhlehwdr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ojriaadx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dcdofzgz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vpqhkfcd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wkqdhjoc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oqqfpdtq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dpsikmtu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nankxqjq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vzuyszhp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2suhifwhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mewmhlop.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yihhwnbd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2raiwvuzu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdzigzry.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2iveeanoa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2shaziltl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nkothbwa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wezaquay.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fodelsxk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pozptcww.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wrdmeuzu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2adrpqxjc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xovteozp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nnhjlfsd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2shdbneyt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ecfdxzsz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqyqikob.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uicghfsr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbuqlbz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2veletfmx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dalzqkap.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2syoysknq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxnfstys.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uuqudjcu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oskzbcog.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xqnefoka.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxuixghf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pzndmcgm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lusvgwpc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cvycvrap.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzepcelw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2shcomsvt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbkijoil.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2npqlwuof.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cwiitkmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ffbvuthc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xfctohtf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mieqyosc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uxkzqvdu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbuzdbkh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2prouvxjh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ijqmywyn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kwzgublg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jmhwkpfk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wkyjhttv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibjstxzy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fbmrnbts.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfpprfhr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qpwvzobq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ufxitfpl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mcyvjmur.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wsfcujjo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2reuhrhkt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qqdtcqhv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2crhqrdag.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wenyybfb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ibbmcgte.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqyafbdx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2heltqega.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pzcljivt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vytrknwd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kyjcpuns.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wtsofudy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jcdrtrtk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nilimalm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bwqkhnup.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rqcasazw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2urqlydeo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jsandrjc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xqzpzxbf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eixrzwgc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rhkpvkay.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2soswzpiv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wvcdswfs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvgqvqt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2puyqgfmj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yrvtpdce.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dyzmspfq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2udjfzwyh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qzwoytet.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jktdrqnn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2iietcftg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xvijptri.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2durskgvu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nkmmfesg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jqyfpicz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2symafyiy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gxwipejr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dmvkyuuf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sphrspax.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nibsmbgd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2analhuoz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zqlbjlro.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cazgtigy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xjoigbgj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qycctvof.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzwmyyap.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdttxok.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cpumankk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gaoikdwf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2grusqygk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kygkkxfv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jimemphw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxnarzm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mcinjnjt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wfqqamwr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mcezkxzu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rvfvjkhf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hrxwqohv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2afgfvmbl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ejdiduaa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2egtpbimr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mrueuyqb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kapddsmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2baljbqed.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xhywmpfj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2usmifayh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dahyrvza.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ojhmghtc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2munkolbg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2cnfbgldk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2awlmdyzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mbxcmkgd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vnhjulwe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vidsnije.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cdyfzhxs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ezkglrsd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pcazgghn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mndzpvea.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2smafmlfr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gmzigpkn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbuxlkbh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qryqpfmr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bmgrdprz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bvtvtvkp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgslawah.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhrtidoq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hpvbrmif.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ifauzlou.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ahqzzhac.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dozmvhiw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zdsqxthm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mdebuose.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gnkbwhqd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xpealczb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcyiiqjr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tsznnubl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sczldxws.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jcattbqm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zfozmtha.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2urxgdyyt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ygnhivsa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wujdxlwu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2luofopew.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cxiqznll.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yhxqponv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aepfwivq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dioedxpi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dxpdgert.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2clwrgvav.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcquxjfi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjardhj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dqaavivd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2htzcolbv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kfdtujjx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hpfmtuqw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mxrtbgik.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qjdfpssp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zyhajnzu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtmdfib.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xwcdgcfr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zmrvjwkr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fgwmbrji.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iyourhuu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jnvdurkx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wgazulkx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hulaleyw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fmbkbayi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2anyaqxea.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jxyxyktr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hrluoazs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kczqapju.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wsaggcdt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2idikssmp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mduloipm.html


<!-- 参考信息 -->