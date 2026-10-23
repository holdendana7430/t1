代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pfkextzs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lbbpcosq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3leoejmoc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qmgudedj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uqqfijcy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3llrczgrn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jlwkzszt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3obzrpcuj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vvdpuzyw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nrisxsrd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wumvniks.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yvpwujau.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hfndczep.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oztdzdzu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zesvhzre.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mqzytuvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3idlccona.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ulbclyyl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ivfhzfqq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wlqcydxp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pdfevqkn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3otabgzsw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bvbwecqe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3esvktpxf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3iremwqjf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qimgxujq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3phnpgqan.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lupiaidl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lzanacyb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3uyjdptuh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxfttazr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tklsntfr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fybynhky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrvkfpxt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dpngfyse.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cayoyxbz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xaelzffh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3iblgvaoa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hxgxytvd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bftgakdq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bywyhowg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dvzasktg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3haefixnh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cbdloljw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bblzcqym.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wednhsfb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3swjuchej.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jmjfstsp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nhwvtxgm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkzykih.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzxiaxj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ugarpcef.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lngolpoh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ufmdqkgs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kvplyclh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3oovlcqbi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qvvznpxl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3poffmcop.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vhokvspm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbwxolo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yvunplsy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dnurpatt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oxefmwjp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xmoyqtkc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3smszzmbv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qgfsqmyr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xaskomwe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nnsspvmm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lhbascjb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xvgelpqe.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3liwmhkxh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pddvdasz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sclryuso.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jmknmqxi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qwntwgxf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3aaqbvkob.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bygyibqs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xttmevas.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hoobufhj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kgyfaccl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdulyabu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmabdrgh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3czwytezq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kesjxchj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vwqnhoon.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bunvjikc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rbzygfws.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3opnuevha.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wqnmmgsv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3snwegcib.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qifqviyz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3akuznnos.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fwooukxg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3verjgnpe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wvvdlgqh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wmbwclnr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ewkxtcel.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qcoflcnr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vapxthfb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tjvalbva.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wxekhhnb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lzjgokms.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dfwmbgkf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fttfrlbe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ejltxoge.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3taxuvvtc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3icuxzzdl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ceaglgtq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zyupdoik.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3doratlyb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nczijrta.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmtgvrl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lebeltnu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ghkcckbu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tiiqbkud.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jxekprgz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cozrciof.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qzdnyrjd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnebrbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wkqjrgue.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ndxsehxf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3usptpkbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yejojvqb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lnakdbmh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ztjotphh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dnuabtmp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ddeaopsp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pbabpkck.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3betlqtml.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rbfblyub.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3sihtliwq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vrezrhzz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vidmaviv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uxxxytyt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mzguikyj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dbdxftyd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jrgjthun.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3poeriapa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mbglmqxd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdwuktx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ixxjooun.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3umruobgb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ozonjcco.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qtqvuixp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pwlnowcb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kxeprfdt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xtdrorpx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gudzhxpt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ekuygcde.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rxqqxlyj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmbogzjz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ffwzfdvp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3sixkcebj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srjnrfdg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kjcqvkxg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gfzexicf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvjneelh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ykeyshhc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jkyfbjmi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tyzeqrok.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zbxdgxvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zlblxbjj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3omqubukx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mupowhbv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3owwpmyaj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pngzdpqn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tjkupkgt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tvvdljmq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oksxklmw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wexcnnmr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3trjnvsix.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jjsmmwid.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3psdmoraz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3venjjmpa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gpqmwxve.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lssvqaax.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rxvzdzjv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bsvzvkpi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ybovoavz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ndpdvatl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3nnwqaqmw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3nwojqvus.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vndjjeoa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ydaqovoz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nlgxcivr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kmshiwdb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kirfkpck.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nqhmnhkv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gylnfqbt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kfjmqwzv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wubahhlo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3txdlftys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfufpbce.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mosqvzxo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vynoeczl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3btxzrart.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3prjwuvfi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xumiadbe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lixpuosq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lzkmmjwy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pasnrjeh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tudnbkib.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ojeagwtx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3aetzwsji.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3awrvzsoy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fkhtxyaz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxagevys.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rsauwbnk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hltlnxzu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fvwpxwqj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aoavhcta.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ytcvxzoc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3stylgykk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hfofnrkx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hqnukdrs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lpeijgdc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yjavetkf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsrstktl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfvxaafh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hwcsrhid.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vwgujhgb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkdbdymh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fkynowbd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fhbwjhce.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mibvyare.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ntilybfn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzkhoab.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3srlymssa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tdkdnbdh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vjmlxzta.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nkuoeusp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jtgpatos.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mxxwvvri.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uhyxzpkk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zjprgnbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bqtccerq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lgjqlszl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wfjgoxnx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hfqqvypj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lsvmsgyu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3skvmdaqw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3omivakwl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vuaaouop.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3raldfnrm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqnddil.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjzptyiz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jjwayrnb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rzueoimb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3enprroqg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mznvkdhh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3okkcixou.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mygoznqb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hgqwpmkd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlkrwwqd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxuwtasz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fcnhtfkg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bdqvzhki.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gznahxxu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixqogobm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqfbkedl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zljvfrds.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ygdpmkct.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ngeldtbc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3trevjcju.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rfdgiuhn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3znyickhs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dpbozwzw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qxkcgnnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjuigptn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jnnqrnkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnfksvfr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kzvnswpq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gmmaieyf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bnssesux.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ftuaowqh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3azxppbvp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ybjjbbod.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sclqdopz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zshwgagb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrdvlmuo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bpxzpyee.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jxreeclw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mqayokrh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qewaxwog.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ccroaumi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gdqpvxfw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3znengdbc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uzjxhqwn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hcmsmrnq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jhcmhuio.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tpbxujfe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tfnftbiv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ilfneska.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3grktvjvu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvydwoj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rxgsxhgr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kohnljmk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bgbpxrdy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3otboucli.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rbksfxwt.html


<!-- 参考信息 -->