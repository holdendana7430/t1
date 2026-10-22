代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vbwgxprn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oazdnxin.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qddczuov.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tznlqvoq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hmvpvvvl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vhihzebf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nvtsbtlh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sdoizjjx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldrxxznw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ngebxvvb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bymqdukt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tbzavfnq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ucamnkao.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dvhscwvu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qawgaafm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ycvavfgr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wwpozeof.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lkvuwfsw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2stnpdsip.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sknmluby.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihyqwcmo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiecdjdn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rkxuxmzt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ywrdzdkn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ffbzbbxv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hsulsbei.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cheeapzb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jbektvep.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bkthhywi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lstfzvfe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nimtjoib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkfeeddt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2foyoijvv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wjjvnrmv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngelvbor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2soijvppx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hdzldwlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqehrosd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hratypvv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jmfmyefc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2toiwodzu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ymtfzxih.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2knmvmxvy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uygeklno.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rosnpwir.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ijsmywpo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2drlyoonp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vmueqafq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jnkkchxd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bdxawpoa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zucxltwj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjmdlpqf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dgczfxzw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxsdikp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ezjiyzuj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lqwsonjs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2iibrsxhz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uaialrkp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2szczyizg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ovywhapu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mijvzfdn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rjwbnobx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pzumswsy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ivmngliv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ahblesbn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdtsnagp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbubiysc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxiavrde.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2caxhcayv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vojzjgmw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2slvxpuxf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2phpwjqkj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2apfjirec.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzyhekkh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2njpzkvye.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fjqbvapp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yxmsrmgy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mypxkouh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mubwpzqj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kwnnfavb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ocrorsbm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pvjvwtwr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vaigzqgp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxjtbnpp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhcbvsul.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vvvsaubm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2docwdfjk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bsxvynxl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cifjccll.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mbujrwiv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pmpzwefp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hxndywww.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kehprheb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2obwjtgkv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kdhjpnau.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vaznqafv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wenzhrwa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrtawxit.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bejqxvpf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kmqsohng.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2snobnddp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kemaqkub.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qnyypiyl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qtlyqmmi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2irowoqko.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2grgklrrm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2npitaaqw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cxibrczr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gzhcufwe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlsgtvei.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wmijmgqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hlygsezm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kbhjzacx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2telnobki.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ivqkknni.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lttewcnl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kjkgqlue.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2paajvepo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oskjmjvv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vlychrlz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lvimrbqg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pedpustu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lwejbwns.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gqrqxmxq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rsuezzws.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ddrhefks.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cctbkegy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ldmjlsmu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zlwkhtvi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uvsysmrx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cyjwothh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rtdklxcj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mpzufphk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2liherepu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qviifqxm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yivjsopk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2dzlxdorr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uavphpie.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mlpioskj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lwrlznti.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pouyzrys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxwzmmg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ogfjgyiy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjfvjhz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nqzhvfkj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fytfwjjv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gbstjtrg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jscbtwkh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2thmbgovw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fhfhottk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fcwvpjzb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ihjqzriu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pnfyfrjh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rdvwobwe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfhbuelm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uwzzogsr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ekvechwx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gowodlmt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obubecvs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqcboijm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nhcceyax.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2topazena.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hkaquqkc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lybiesgx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dfchohch.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fisjtflw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjrabjcq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rdmvzeat.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bhibjqvf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2drsncoos.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2addgkofq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ggudusim.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hmpzwpxw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zqjeotpb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mccwmpzn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vdlimxpq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mvylueln.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lvyikagp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zpinjtbu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rrqcvkgz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jmdfacdm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bybdcpgf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fptmqgkb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynfyixmi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uhazozpe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2niiifkzr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wbcfiryk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ztcdwunz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwcsxtb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fogigvnb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2netzqmqc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hzfweget.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ckuvrnpy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yvboydob.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2blnckwin.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vmvfzrrz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ajzptvle.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2iijmnaub.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tdcyymit.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxsvsuea.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dxdzbhft.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mooosqqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nsxikrez.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2koqylwmh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xvbdexom.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qyuwwiez.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jvnsxyzd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ldogvbyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rlkuxjeh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2trqwcijv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2afjtycew.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwqjhdju.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mgosagxs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aoynicqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pdxpdcgy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yhhbtwhi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ecycycns.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yxrjwala.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2iozyqryn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ftpeqadq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ipzeflew.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlvgtsm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khuknoeb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2clexcliv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2csszgyvy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxeibcuk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ogaubyau.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fitsjshu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jqypepah.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qjzmsjiv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwzerlmi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kxmldzeu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2inpfhnxw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vbxylcgu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dxzegubk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2szrtwvuv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qttkwewz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gkchivpq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lwwmfmiz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynenigcg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ooglohka.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gmddhzds.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uizrewmg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2prwekkiy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bcmbusdx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pqtgrjgb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vpikcawb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gynzfywa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wrcjplbv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bpvcmgim.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jskvxqld.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gnumghyr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2omgtflyj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2irisihvd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hawkxzed.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dszkywmi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oheqltae.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxqtjag.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lsweolbe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tgshyvid.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qprhrpoc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hatjrhuw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2esjemmbd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2msfappkm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jesmjjxl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bpokwmmo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2etsixynt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zhognjcj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxjmbnd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tjbdfvwr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pdzddfiz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jkuydnws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dymdlbkc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ykdnqyov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdntywex.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vncsrniw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zzabkwuw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gzwzxrji.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kwlpkbpu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ohmtolxj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fzleljas.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vkflwmgb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wzdkkasr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhjmkpyc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gmsxedxk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gqllubcy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mgksbrqm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2chpbavws.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eejzzbib.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2epifodng.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kowoiixm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ktgqsdva.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kqjijxll.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ucjqbtau.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nffsehrl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2itrpitkd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bdknfazc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2odqstaif.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oeakkyme.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2baiepnqy.html


<!-- 参考信息 -->