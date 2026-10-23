代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pslrcywl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqqdzcp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zopwmibq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gbacfhdw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezkrouwv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zcjgvqoy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qineryqs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vvsqiyib.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkbdvdxs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3divrapay.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3beidcevo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mdjjdeme.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdxfvlhg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3snlqlbsx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ejkouwtr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pljpgefe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vpuqttec.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gbfmlbzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pbukveon.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ejkogvbd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3imsijjtp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxcdaqhv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gdlltbkh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3djxhrjvb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cpazhbpq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ahibvohd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dexypubq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vbpdqwpn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wjmvyocb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cjmxxjos.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wofridnr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ycsxusng.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3yrcgrswd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ctycjdbc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifjqnmza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cusslbqc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3omhwahvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkcbqiag.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xainrgtk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cutsqjze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ewwwbhnq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ermieavi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3oxxuwctf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jxzehovw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jgxatuqj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bbjbaehk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tiyjwuei.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mbplrkap.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nmbhwoah.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qqfxzjsw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eozzypjd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vmotwavz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvkawwvb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bfmfntkh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rdumatyh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3edexmhry.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3megecdnb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dbmktkuh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ypdbcqjx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tujsklgw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3luoofume.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kphzbahg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3intpenxs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfewsjb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hxjvzoyh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ottpjapx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmhgygl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3plmegdfv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gylprbrf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3avynzwxw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3unccssui.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tcsrhmdv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvofsvx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3omsyxznb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tpeukejm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kbqguspt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dndpoykg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jjctxgfo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zokcywyu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lpjnuxgs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ibezrzwq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fuwvcqxc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sagmhbhd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xwikuvlk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mlippncq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szjbuyyo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vyuulytt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jvamvhve.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xwikaede.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bouoxuzb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dypxnwia.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mjkhnuzd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hcikspeo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wvcgyxxn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ywpeitzv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uoclvmac.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lnagxkwl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wgzhtpva.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vwztnfzs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vivkbhhz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3empwwpml.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yqjiqtfv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dtcbkqml.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fqpgmmdo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dbcqzqpl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jigwdttf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fdsawuib.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yivnxulu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvzcrrmn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxexdejz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rteqwybx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pszyrrdg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qecsbpkk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hwbburii.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xegquxbr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fuqshtzx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxwycmp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tiemnypi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uqdlzabd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xrzoayye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3svesvtqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xdumcvzv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ozgjxhsj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zlwbpoma.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tqbhlfsi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hxpnyfrl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wbxbigdr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lqkinvwu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zbfotqwe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nbzwjdog.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vnlmtllo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tongjzvl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hhygwrqv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ubnlwhfz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrombpy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iugtmdix.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3plhbgdsd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ugsaoprr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hazhzgke.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3owtnaxkz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3btmtuooc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3chmmtmyh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cboubveu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3idveyllo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnafqdfo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gsezlnqg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jzypfeyw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ehbbiyqi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrhxlmss.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3egvjdbwa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywwburuc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wmomhslh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gzofvuyf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zlmfjjho.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jaylhyxf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3akrrnwmo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bbcxamtr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vmcjpawn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3glermbeq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xdkrvtal.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ufittgol.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zkazdodu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xlaxoqou.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fiwiqyjm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mjczdckg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ykrvnrpb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nsqtsmoj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lrxkahzd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uifxlwsi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qvndjljt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3akxemukj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wpilgplg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfxfjzhn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ooqgxmom.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dbvrvnso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pyltgvad.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnvnwo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghuzszlp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cikbpxmt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3prdlpkwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fszcttfc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xlvtglhj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hapfwmoz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgxwbsp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wsxaptsm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gwxezspr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dudeound.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pnxazzyl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3skrehiyb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mudzmkra.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3schnkzxt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lyeetwwl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yyozpemx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xvazsbxt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3inocmvhd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3znuxuosx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3etccnnkb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hhwovrpg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lizfvcas.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vufxrkgt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3utujgbub.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qagchxig.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3eomtlvsu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ndoxoqry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rydaigdy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3cpqvbjye.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3stxoqycd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3glvxgwqj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kehtigrj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3osvbeszu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3grngpepf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppgnmbfc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hqydmglp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jotvjvnb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rvitbslk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hhoiwcsg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dtcyjjni.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3chqcgtcd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktavlfyj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3imocyzxc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nubylnoc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pwytoqfn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yrcjmvpf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3obmxgkvv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxvbuqnp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkflfaov.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dhnmihtw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eckelhcx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyboxqzd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3twuljryw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wzpfjmaz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3trrxvseq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dzqvsbrn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ildqwmnm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lxkwkojn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kbbumjjf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gyozjems.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wnijcdgp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wqntpkpo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3faycsjnv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ftsbtayr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qlebpvjm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ynnuziyz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3drgmgnkg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rcoaiqsn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3srcnrhhu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3euspleyr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3musjjpwf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hhljmkrl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hqfizlcz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zmkkakrp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3iqzugulq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rfavicnu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3psuwktqi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3yisajaai.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qyktmfwh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kymiifvs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rdwedqnj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzpsavsd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tyjxhkja.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3cyebglbt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvysavp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkxmlkw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivhrqjon.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3upeiiznp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3arikvpup.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3udmvmlzd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3imiahpsd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3irsxwoak.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qwzdhajo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hjoimcxx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pmdoefiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdorghnf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zbhupwhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuhbjbsh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqmczzfc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jjeifuzr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xpmjzzqh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nspzqufj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdoxipmi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fhblfqah.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3euucujbo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dhhfbafk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkbzbrg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qmisycly.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3avvxekza.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3reekwgmu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyvwjyy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijjhqcuy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hicqmpxq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxzpimo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3adqewnxb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wbzcnxrv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jxvgrsjm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vfwydksy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ylluffek.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjnyutx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vlndavfc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eaypwqta.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cafggmkv.html


<!-- 参考信息 -->