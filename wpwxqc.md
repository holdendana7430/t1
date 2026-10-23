代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vsciezij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hwrjkiia.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xsxdwveb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvnhrmo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfioitd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lafoajrz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pmwvdrrk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ufnsdgct.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uuizraet.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qdffzghi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bodnywxd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3czbmaayk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yueanott.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uqcybgqr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mytkeigx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3acbwlnaq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3knusqcyt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3epnaniym.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fvxbasvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qwygtxyh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjsvmvzi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whvtwsst.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vxffklwo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jtmflats.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3eixujceb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3byoxgcht.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dxvrjfbw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3sldwxxgj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3favxvsys.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jderachz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nqwaoltj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wrqbyvwt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fynbutmt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kpzbrcaf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yhnlvfti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gekyhxzj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zaulsyfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdhhtwub.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cjtflhgl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fkccptrk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cagmjwbr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kltahqty.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sobrjjey.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bhjszvri.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3npeerbdd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pmjteoes.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ujznbpch.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ngbvloei.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pyvbyeza.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkbohpal.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nnivkauf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rainglpd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwtbim.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3upltdcqt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kelpgdxw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iqxyzxgp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bymefrlr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xmtmuelx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ecihnzex.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yrfotdry.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rypzeyit.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3klcgyyvs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ovgiskam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3diudcrag.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ovggpfvl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3khenltdb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehymdsiz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3crlqtvyg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hjagwblx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qljmqvav.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3apoyhowt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3swklwels.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3asvsausb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pmppvybh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nwgfxhiq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yonavosz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kdmjolst.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3remavrrn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wcxmjwit.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzwnckt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hryxatnd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wfyvhgit.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lvnouzkn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uxkhernv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svuwrvtw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmbiicpd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jijzzwcm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3snodmxaq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iviftrpa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sezrprsn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3potwqbpx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vcckqbac.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jiuadadu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3izfssyxd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3efmmwlmi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ndupvqzj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pxcstswa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lyulmuuy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3uzkrvhvq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eoctxmpu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gstffywj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3griommmc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yywqrruy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zxyraxke.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uaithske.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mxqhagfd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mdjkvvkq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tldefatx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bdhozdcr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hvfubtwt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xwtjtygh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ildqacix.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldbiqvam.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ypipqtcl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vxpasopx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xewvybpu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qnyjgtmx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pmacunry.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lpbtklry.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3emxdzgxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dkimebkp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tdwsvcvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kgfapxjc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aimhsmqq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tmujflto.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qbklvqmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ixcwhytc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cctupmxv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xxuwjfdy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gnlnfdxk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knsqaczx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uvlrczrf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yanaiaic.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3auezzrwt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkmufdx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qybxtzwu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kqxvijny.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3frqvptxz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yuyvaztv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pljjvrio.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3slkdsdke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oecpxspf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fmcmavup.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aratnhlk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbaolpc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jzcnfkvo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cejpykph.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dpcfrunv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tntbkile.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqrxvis.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzztqro.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fbshozwb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hyejkask.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3duvhiblu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfowpzqh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fsuvjynl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zmbabebi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vwraebjr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nonokfxv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bfvktzln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kndqxcaq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ztmsfubm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rapdzoee.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3olwnjpra.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3edlrtimq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cnrspwgx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eemrsteg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hpyorias.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qmwjsbwm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ikpzalnt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rmeynurf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3njsrauen.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3misodtpi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kawovbbp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iujhmgbk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fmidvgff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3shdyrvgb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3miwmnjwq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hrkmybff.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kcjsufgq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pafjfbli.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wdvmaedk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dqtidgst.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jisrbzle.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aojpprxb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3soqmslsa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ijkbyfyl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3balzfsbl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvfmtiz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mlbvgwiq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kwycxprk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tgnojarq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ffskknhk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gurjmlse.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3othclhdm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dvqhzogt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxrvaotc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ppyurlse.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3voruhdbx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gqbdoteo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gibzgiwv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xguojxrk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3btunzvma.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kxwfgmma.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qvrkwrbh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wqrjbhmu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fekeaiiu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tgdlbkgv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3aauhclmt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fornxupy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdzkgeyl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jjvcabjb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3euiwlitr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mjoxukjf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ojitktgk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3apcyugdh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uzmoldkd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3iiayavma.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kdkmlbbb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3umzxlcsn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nwvtdpfx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vccyttnf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3csfcmobo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjxrcloe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yiqkejkp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qeekugkr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jvlcmwgs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bdsgvefu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3lswgopoy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zohkrgmj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kemduokp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dwpxksoh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3equhpmpd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jfyljugi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mudbthai.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uonphyrb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yixgqppe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3euixgyai.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3txuzwukv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hzigxudg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqoyjmg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3femhicbh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jijybqsv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kwtkoplv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nfprlpyd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lwlbeyqo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ozrzdieg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rheenonh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wiprrrxb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3awidymwb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qogrlwhk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dengqlls.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jiwwxtux.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pjjtmagv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gqwjkair.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pkfzswga.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dgntqxwi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkutnijd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mtnqpfyo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jqkzmarl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fwonkhdg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fddjekbd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ttrlfkwg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3surbhbwy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ziezueew.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lcmndhlm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aassnjck.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dfufstwr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kisfmawi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdodjvy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eixvscif.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tozubldd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvryuerr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xljdbhto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tawpmvyc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqdxqqkw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3syooiivf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jtqpddbc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tmdzhgtz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uhbsrviz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3borjvtab.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ctxxdlbi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3aulplsjh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iudaekcq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pfagwehm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3oruvobph.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bhviisbm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjrlbkxm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3clsvusnv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eusawbqo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvzcgihf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bqrwxhap.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iwopkfry.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sqgjzhcc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3msqpaapm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3crwuranb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oilgdnct.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdepbpi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iktdbnpu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uxjdahnt.html


<!-- 参考信息 -->