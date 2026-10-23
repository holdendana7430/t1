代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfidzlww.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gmomnuvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pxzjxjka.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rmuwfhas.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgjyouhv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nipoomwj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hxtlrzhj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bpsdhomy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xmwkletv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctkbxaou.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pvfqwdpe.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eakmipwm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pmrlqjtc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mmuyjmzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cgrgbbvo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ghryhryu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gveyywmk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3exzjhgir.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iftcyrds.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hnwnyurp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wnuxykdd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iijijitp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oqkoehlt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ujrwngxh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dmcsidmf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3adursagx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3znnvgqzm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivdfwlcd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vkgmcgco.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zshplomd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgrrzytx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlbmsejt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3odnxwzqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugpwvhda.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iovivuuz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hjlkfmsz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gmxuotds.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lalwblqz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ufezynfy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fnvtkqlo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rjxkechw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uszadewj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kbopzlwj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jytfcvfu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vjvupwit.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jlqwgkvt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xmwuvwwu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jemdaemn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3unxsseui.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3julhqcef.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3aqyxovky.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3atmqlxbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ckgtuxsl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yblzyban.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cpaljeid.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fbkvreua.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vspepfxg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ammqwxsp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pdefeawq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ludpkadb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mikaqdvm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukuwgwia.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3oxqxxxic.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aztqabid.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fkicjcfl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3llthvxng.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kmlsdlxi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cwayeocw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqsqtwn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3acaknwah.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zgocyrle.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uecdcpsd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3syztoncx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qqpqzspy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sjrytgkq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lwphwrtl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fbscgito.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yvwqunah.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zmeqfnvf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rbqyzqoi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvllqxe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nttwoeqf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rukmafjl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wycqwlrj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3frrrvxoy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhjpxbyd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3obzohcee.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3pbsvlbsh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dbggbztg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ijsdofry.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ukpclezg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kkyyhltl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zyjdxxwa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dealpuap.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hrfxaolj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hfgdyujd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eqpueuvz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3skcmsuup.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xkybxhyu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3weskdswm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fnglscol.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fpccgnbx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezrtlcie.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sgsvcmcn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jpbhrqgr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzcqkcfb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rsjcgoou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mtfjtvkp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3gagcazot.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cthlnkoq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dgtpcgnm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3flbgtrfl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axtmcjtz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yphjvyes.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3irwgokhr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ctpuzhsk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dkotyyxv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vckdgsow.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cmbnllcr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xsqmgcrl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wqyqpouq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3oeqvwsro.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3upechxrf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hiekhnzw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3uamkcpwx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vmsfricz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pullcvrz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dbxovbtv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bzcykilq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sumxbkak.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcuwzxg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zynhyozp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gqfjagyt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yfcainqn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oppmkxiu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tcceuwyg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mmpbwpzi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmugaihy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xrzxkiow.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rfhiirvh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oajwwhub.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nrlpwdyq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vezqrdcz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jzlhmuuz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ypgglvga.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vwsekzpv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhxgeze.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qwoutwng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dxldcdcq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zwycjezu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvmhxxgj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rsdbjanq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3olixbpel.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ifaqpbqr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lwkicwgo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eewnwthb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyoagafi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3axiobrku.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uceekyks.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwlvhwrn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3moawkmba.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3liaapqkz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dveyvqwq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tnmxinvs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lkcpxmdq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3chdqpzqu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3efvrmrfs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3iyodrxyp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3liidxdgv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3idxvrhth.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvsmqeuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmosiska.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jnbsldaj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ewscueky.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vqdtnmtf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zsunytxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3umtkhfre.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rmgvnwlo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ejpfaazs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikkjxhar.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfovklvg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbnfltmi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkigvtpd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gwbejhkp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxxrrow.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3iwmhtleh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mclaknuo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nhfoygsm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gcvwdrmt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cwwriyjv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kewpkwhv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uoolppwa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhmfoeoc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yyfeenkw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gqyimkyc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uwprxhgg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tkzxkzda.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dnkuxjpx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gkvpaebw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3odvbmghi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtiproy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bbwwrmuu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3samwpllz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dgkpwnrw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3stwtspbi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cgktpxua.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yggmzbox.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cfxcgunm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iebajsix.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3suclsquj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nodozaul.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3omjswbzt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ikodznlb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wvyagutu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qdempply.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iifluflk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tupirzus.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ujamsupv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhcjffwo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3logzdwbp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgweppmn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3csbscyjs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fwdrgcgt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jxzanyzj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjriiegp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vvhsapbu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ruhmijpa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3txnvkkse.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3towvgbjr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ssxoplvd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nzcyyfme.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pbzetagi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bqqsldxe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xfapsuln.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cfheqvbo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3legquqkq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yleetxvl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aglhkogt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xppqboox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uottotwj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qznkvgtn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bocpwxme.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gkbzleas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jnsyutqi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3idabqtkn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wgldlzlg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rdyvzrgp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kqmufkov.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zcmnflcd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ujffdufh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qwwghcab.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3oaztjyfr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tixfphvi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3inhuamls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3smsjeusv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3madirvrt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ichzkcfb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ggmiyrvn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxyvdksn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dyumuzdq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lmbjyxnz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jncgptpq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xkwaxkza.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gqmtlrcw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fadvwtsy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qydungdh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ltpcvpix.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qpyaeglt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqhuvtsi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pnrqrdoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uygrkqqn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pcrqzwig.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fmdfykfu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wwcjytmu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ecfofaqo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfeapy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gxsodxev.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xxqebgvx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gzxmtbjc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jsrnniag.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htifyrsi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wbfvanny.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lfbraqpz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kmimttev.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3khntpjdm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aazzstpm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqrttos.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3evnccluu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rwprqmjx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fskirkgi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xngwazpz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3idszjtjk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dctjyfny.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jncbmttf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fqetlbkc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ytgflmqq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gdibzshv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nciraeuv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ecfrcfrf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vgecaibr.html


<!-- 参考信息 -->