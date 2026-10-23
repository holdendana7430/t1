代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqhqrchi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ouenirou.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gxtuqllr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uxnajmiy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ygegqgcx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgyqbbkr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kteollzq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rpguowsd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ooylacpu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ynnmegeo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gdcmqvmp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ioyamzvs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cfiaahmg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkywxgdu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hrwooilk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3exnhsawp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xeboanfc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3taicbypc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dhjvaoeb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wdnsaqil.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3sadxtfqr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dlwubtwg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wuubnasi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3arqkhind.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mgpeszfx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztdpjeqn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cjndshtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pobvvbov.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hcdpojad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iritkflx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wmeyrqwb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rmoxrjnw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uckakpbs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ylqjbkjz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dfinupkf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3awusehoo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vjgtzygu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ytyzbvoy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pqglsxbi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ccvlhzqp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ndcyxixk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rrcrjsci.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tyjugdzq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cteghmoc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iykbyiqu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnfenluc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gixyvlau.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqvnllky.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wgbgkale.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3epgqpfti.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzkessgd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tcdwtowk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xswlgmus.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tpexuvxy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jjkuaxat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jkooftyl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vzpuaaeg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vxbedjoa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3owrbawzb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3asjgphsk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uvhwybjx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tnbnzzrt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eispfdzt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tnooqqve.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xzngtwsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3geimjgur.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ymjdlydc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ztuqqlze.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vkksxqlh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3shrsdfen.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xnpybiok.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ndkaljeo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cucwptua.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3slpfmjfm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uitwluqu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqtijejx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zriafyvt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3taogtfrk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mdfhiydd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pjvnljmx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jjpnmpof.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxukvfbh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kxyhuxna.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rhtqkpdq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3brckjizz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dkqogehd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wmpfobgn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3egzryegq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bbhnsphu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rjejgwky.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xhigipkd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cjlrbeug.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oabxgmfw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3psvtxmcz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bcsoaiiy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zxolwvms.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3evfpqrpv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lpegwgnw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dqcqmkbf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xijwcvut.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gioqnqhs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjgggwbz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ljmfretz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3owszlsng.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jruaailm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ytrucumz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3doxotavr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3naicietn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwgesrnk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kfusuklt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vfxzmznb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nswhhmgs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3escrlwfj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iblluzuh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lvoxtzzo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3huchllbu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ogoayfpt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rdzuahnr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mtasbskj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tcuhqcil.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmbbtmah.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xzjqlhom.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdkbqqzw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cxuxdmll.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hpentixb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eetynhwb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxdojvbj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vshwgvqp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dannpthi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tbychcki.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ismomynr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cczcejal.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgoecykd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hnxcohgi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hhzztxfv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3babrixsp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xvgdexfz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tgwhglen.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ibnqnuef.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rozmfauj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vtzmmuds.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3owzwjpws.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yusrtmvm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrkxyodr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lwjuxtbk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkdjdkqt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cvmawsxo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ypmuxfpm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3madgrepd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edseqoje.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fiuvhmxt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ufafxase.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aynprsjo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3okyfclcl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wfavlfoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3phdzybpb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3avhzklvk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3crgfiyzf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prdboazb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oshcjknf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3awjkmykg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3safeilwb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3evoeugwu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jbftycih.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dmmfvkri.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kbhhvhjw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iadbikuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ypzffqbw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gxondohk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ykluyrhf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fjtjvpgq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3imneeywe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wktgquxy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uqoqnjff.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ldwwqzik.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3occhzioi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qnactsdi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rszthqxr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mimzaohi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3besmbruw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnryceeg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nefqssuw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ensempnr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3axukmfsu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ddjifldt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wqnbnrwb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ubwxxmzu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ifdfdahs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ohuvndxd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3aoaqmnhe.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xfjskdoq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3anrdixns.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3auglbgoy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emsilzev.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bqrfipqd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gowbghqi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sjpaezfq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3afynbhag.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lfvyrjac.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zvhddxvk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3twugxegw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fwgimlbo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fpmjkuva.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tutbjprg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dcfbxkyv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rsrqwwza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dwjeurik.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ivlefcrw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3noovicou.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gthwdiax.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3otfmhupk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lmijswev.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrdxdsy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgdpzpu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3isuvgcez.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybamimut.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wwbdmxoa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eojcjcqx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kxorlfpz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vdtblcmw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmtuuu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oolqlhsn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tcibmtwe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uvpkcteg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xeoxqlgp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3duencqcb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3egkimhnt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zshddsyd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rkwqvpmv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbyvhujx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rmelewhz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uovyhlwz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3liobasjy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vfxhceeh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dpsnbnmo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wwnxdukr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfnrdxdn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kqxrnliv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sabeklko.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3niltwfkd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtocuci.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wluqnyee.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxsjbscs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vetbifqf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3djppzlld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dqvoceue.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fagmygzb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zytbkhii.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3izqrbbsd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jparmgyc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wavyxlii.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rboxkfed.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qorzmumt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zrxcssnx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjebgxpj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mgdgjmqr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cufzohzr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hnrbiaeh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kruammsu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iwozoyed.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvcbsli.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dgacxmbo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nwdopaxt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyhoqqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfohnryz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pbnuando.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxazdegr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3blzqoazy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rqvqnjcu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xkxuwkgy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lfghccji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mldipiiy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pllwwjat.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tgkokwmw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cykdogjq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqchkxno.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cshfswej.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3byezwtwi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wljowmyn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hujjlwhc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3laihmroi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kutdnkfc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbipijxu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3otfgxbir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3leohxbxk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sfipvumk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ixtcoimg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kihxnxcs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qhshwlbo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fjkvoazj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qxqwukzr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dkapqfbn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ppgzihct.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xvvnbfnk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fdebkpkk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nxgekeck.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xizwemdw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3adnmzgdk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nyavwqfw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqwlkcwe.html


<!-- 参考信息 -->