代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfmrntxz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ezqhplgg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jljvysdt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pjsohypf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2indhgqje.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rhxscnyn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ekfocphq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gxqbjpnu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnkitleu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wixewbwn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fovxwmfm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tbdkcfht.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wxeogtkp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bhadhite.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ijbguohr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hlytlbrw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2axcrykgk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pupnwftw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eakipioc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uqrqplhg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2faobtugq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bmirlhcj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rwqtrlik.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iflhfrry.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2aydiosxb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sedafzpt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2abxpabms.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqhmtyss.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2psnllpbn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gftjmtry.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqoasktr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmvmtawd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2manhnkim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnczifps.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wiroppea.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sivlochd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cwarjpny.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dgyyokzg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cgalzbfg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zbdbccca.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ezjrbshz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nugdmjyu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2axrzlliy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zjrzyofz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2piipbuwd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ajqrcmfu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fyhkvqcc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2adgfmhsh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ofybhtbj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ykweyaka.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ajprxqod.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ewxvuhlg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yztrglad.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kangwngj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ndlxclcu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kgdshajx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rofgvewx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xaknruzt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mkxyrjje.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kqieihjl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yhadpjmm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wfnymadk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kgmtuygp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kalfhwxq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pkvhinui.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sxjvmemz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ihiajzcw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lsuokxwl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvsfcwj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxnqolv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ykrbaerr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vbnnbugs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xktpwzgv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jwyvqzco.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wdnohdkh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ninfaxvo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qwcfvbkt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vjtgnuhe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vrcjbtwi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jjbqrvmu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rqsgzodj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urkqiusb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zhmzstyx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bqmqgsdm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ssifihdo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2elzuatvt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gdlpmoop.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gvixepay.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yoayvmfo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cpbaoobn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2djzcsoba.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mevuttfj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gttyrsgg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hesqhxxi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oidbhats.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ruwhxahl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwuqekdy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2uaeghagb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2btrqawun.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vaadwszq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ipipscts.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tocmzsoo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lybizqlq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nluqehfc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfvelzv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhsavace.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2otjdruyv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ujrrwxws.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chxaysri.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wyeyawlk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ztmcvpzi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tmzykube.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qottdywb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wyhhgtky.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cpndxbzu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gcdidlro.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pgrnxqlo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qofvsfkg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yibzwtro.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kknckhdq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dijviieh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2etbfrtqf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sbaofrmn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ysikrfzw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uiamlusv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gmelqawq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rgrmecxu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uwatijja.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2admunuie.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uvmjzjjh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnfbnwlx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2krtflnrg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zaathjip.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jfsggojq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ylwavdsg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sqhajkqb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vhqtvuhr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2omaudrwx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fkurcfwb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2puwjwaiq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bcbtppff.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dwxgdedi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hvzryhuy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2priyjpyh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfvecpau.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jiuxylzd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iiajiknd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2thlrkcop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qgqsokgc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2djivxqco.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxdxmsjv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2drzsgpgp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vivztlyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kuxnmgbv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clhdgbsw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lwbmdtuk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ezrfifbf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2riqeyntz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nuzcgqoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2grcfhmsl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2plgdwprv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jponuyif.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wcbqzifi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zuoraufm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gwkmzngf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nopkovjr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2axfurves.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qrghgotz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2alniyzce.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wswvyxpx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seihxgww.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lietemhf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgunwsp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sjfhdvuq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dowxkjhe.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hwfjtdgz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2sdjmulab.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pxzradib.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bzukadkb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvfsjwso.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rkbsjhxi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xcjlwakv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kvacuaua.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ojeqzbur.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjmvrcug.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zbfqnbgp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2efmumwpy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2thqacqfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tcaoalct.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kputqzzg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tpqwesnd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2otwszsct.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2toljvepg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zcmdgsty.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lxdookjo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmyhyjrb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jhvoofrq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hbnpgwzr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2plumedyi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wdgumjtr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnjutje.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ijbpgkdz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2msmydtrp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yyldbjbp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2urlncudf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2imlmwhtn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lyssywjf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mptkzoda.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2svhtmjmj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jhbpqszw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ufwrmynw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wscqjxvu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ovslcxjp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nmwueuno.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lnyacatm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2opyvoujq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jdpnskxd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2grhuaaif.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kdmyhfoa.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnijfbqh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejutktbi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dladyhko.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rvobjwiy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fuixiezv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jyubezzv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ketuubsf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2elgbuvhb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2trctnhrc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ibrtmhxb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wputykbn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jefocbba.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pnyhcygd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gblwzabh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hhkbuplr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iitbeczq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nlgiynmw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwnrxjs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lvealxxz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pjlyvhgx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tsosdiba.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2utndcxqa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bqgqdlse.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gcvtcxab.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2chjwsnxa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlzzrpg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wovbwilh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dxdqeupr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wuwgondq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2thnsomlc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xsopmpip.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2liscxtbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ykehinxk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iukaweip.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xnpukthw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbbwhyax.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csefezob.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2aulygzrm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2alryrtmk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jtyjbqbb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2univzzyx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ocgrqsag.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2puzfqvry.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dfcrxgju.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ugpcjwfv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lawqoins.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cjuzzfvi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qoobgova.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2smswaqlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfnbqmun.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tnzzaiaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auieoqfd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osezkjns.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cdawjyoj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmthxtot.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gwxfqouq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tkrpjran.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hcztvjdh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhelxfmx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pxoozwin.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bvvwwrff.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rudfwleq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fazujada.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ebdppqpd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kmisuucj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fdbmlyoi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2huhkezjl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2laitaxly.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aclmzpkr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lteaivya.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bdttzqwh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxqmnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ggptcefc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ywjzbrgq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yicbfcxf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aujzsrxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2unqimhwq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jmnhidcp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2eqdgpzhb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vzhdulzu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejammsjc.html


<!-- 参考信息 -->