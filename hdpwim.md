代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2emmmgtat.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bmcawayo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ygfeipzd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lfwsymre.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fzvpeqtk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqilfbgr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2avkcfzaa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jlgrhrvg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ffxofgzj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ibgywrbq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ouhlmeoq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2izpwjvdx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ypgjppnn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fgkdqfvh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nmqvzarf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdlmkgkz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yosvuwnh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxsgyiqp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjscwnjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uywaydrm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zihjyccd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilmwsayj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hvkmgijy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ranvpxoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mxessdar.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xnibtngi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wjowbfnr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kjovjwmh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ifddlssf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2iycepegw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pjgayxja.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2owtnydna.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jhnggfgc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tcfjrrmq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dlitrmxj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cjjmiurf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aqfidytq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dfysfmwb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2byeykwbg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zahllqde.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mgjnncir.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2aojtumxe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wairptoy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ypzwblez.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qverveba.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2loujynlb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ferwoqtk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqpvrvvj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oosdxjci.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pjxfsxju.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2erltcaag.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymhqsgrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yuvwdckv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nlhbbins.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rklfhxda.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qnigezsl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uirppkit.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hrboaarc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2erwguybs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zpkviaih.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yzqlcukp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2twiapflg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pzjhnkjs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zwivtmfu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2guhtzxqw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mfzkbnty.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tmhlmdel.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xwmpyrib.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hqkmrtbl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cewvxxuz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tobzzruv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ietvrdyw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2flmamwmm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2znlskwwo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gzgriulf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xedudgoe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wuhpblwc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2igdhwiyn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2itkkeulg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fbudbvzl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iymdduyz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zcobrpxd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zgdaqkld.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wxtwxdnk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2inyqnadr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yxlfhhzm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mvxeqiax.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yxtthgde.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wuhycbew.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2stlarpet.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qnvaxffs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ivmnqdag.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ecnrvoxl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2apiqdnvy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qtbkobct.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bfwadque.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmkrybus.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lmqaetmo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qktpehqu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yqnkstkp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlystcom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iyrskjqs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xbpbzwva.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bjymoqji.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kljuggsz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wdkvivjg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lgvrffpi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zykgikkd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rcdstwvl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2owbgfwfd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lliwtvkh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zotolsmv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2slvbcqqi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jhcgkupw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngbdtmbs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jzhrhlws.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nvtvvzic.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kvitkdkh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uvqaulqg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2imbnexcf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bochvgef.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2raefdjnh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wasyskqo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2djqofpqu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tvawvaaa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmicewu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ajigochi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jirhskhg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vvfwqdbj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2coteqkuj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tlaenmke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nszwmsej.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ubiuudqx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgedndug.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cqjkydfz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvtsaxcg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qveplxmm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xyocqdhv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nifimrqr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fnpifppc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zxtxbzgj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nsuhmafv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oshpuzcf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2faffcvst.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkwssbof.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pqgivgxp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jattoaky.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzaomi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nghkkrox.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhaudgjg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2viiqymqa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fxmnwhos.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kfqxnmmw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2eemadhkc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gnqlajeo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nyjuzngj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hycjensw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cecgzhub.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhxycsk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxnfgbdu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dctqdxtt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lpcqqjlq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2znnxdgtn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2avnbtczq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jozphnvt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nrpxgbgk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ugimumpt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pvaxamim.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqprwibu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jeeasdca.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swxgofgt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2awakazjf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rerhrdmm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pnhsdngv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pzfqsjtz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ikxachon.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jcfgmrkg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wtzggmth.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2srxxadse.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lvopzbet.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kvhprsaz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrzkerqi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bvxhklzp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2heeuwfwy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bdrlelyl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsnxmcfi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ahfqgswn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ohjwjmef.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2edaaywqq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dfjeytzp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ihsnnepd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uucnqyia.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zcyvuatk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2skafglzz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2clzdpnzu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2odpvgqnz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cepycymk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ucgglvbk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dnweyahi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bycdowvw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qdsyrxsy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2piscfxpy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wicznsio.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aphtcyvg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jnwmwzum.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2waowpymt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pykrxkry.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgokxbml.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdibqi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nxuikowu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgmtrzzd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qzxqfpyj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgvkespf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jkztrmly.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vchlsnwz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wyztctua.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gwepeufy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyhtdrj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bbvwdfjo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rvpdgzmu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zcbpmuhx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrionqg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fjatkuic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtmqrdz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2guyetqgp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yxsralvo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qnxkovys.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ynmmluny.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2npdvjbff.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iwqgdrmt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uvcchpta.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tcfyxqdu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cutirphv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfpasrds.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxofrbyv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fcqydaui.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2izmjiuvw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kwfcrzdc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2idkbgnoe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lradqviv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tcrzmenr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2airccmnn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bgrizuiw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dsmwmazq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fhkqpogw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sepytscy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sorjaqeb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hvbkztex.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jtzdeoyb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zpihrwxy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zkluityk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gezcjpqf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bfwqjnja.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nzdooxkm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wrwtbxoi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uezgcojm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcyqzvhw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2lieuvhgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhpojeav.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2elsjzdhy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ozyrrayq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yhdffgwl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oodeatcl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hfqkzvdj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2obiwczlj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2blklluge.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wkxvdtph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rhhoosyg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmzogrfo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cacepwgo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bjrelyzq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2psbjblzj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kfdhuhhv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2anviqymj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lhurbxwz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lirqunzb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hfkmntif.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oomrrzdy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uvbioudh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xvzbwhkh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fulsgwcg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpnvahmg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2donlyjnd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2imzvxjod.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wncikuhz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qnihrxrj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cnwyamfd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qbwxrdgo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2behjlpvy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tezwpztx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ozvgobsy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sdsbwwkv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmatfhiu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nmodsayo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2izpghvbn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2sokgvmcx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqeaspz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fdwohgdx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zgixagia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dxbtzyup.html


<!-- 参考信息 -->