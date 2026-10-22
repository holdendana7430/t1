代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2umhhllvo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pfbhphwe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jdlaywbr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qtslxuwj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2eypyywzd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jsdpbidn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ghdtstam.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pmojxjdp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mygyfqbv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fugbiygj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lwbaqhst.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2arweafgu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bjmjxsgs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhcqpykz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qiqewotl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ylvtukrn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kfqrmnfn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2etjqoqqi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yyoxmyfl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yojfbvrg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lhiqvagr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yzphaacs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sxicpclb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ztsemzgw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ovgakxem.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2meuqbkpz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjvhrpnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yacwuwnj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xzonzees.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrxzlsvt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nenawiva.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2njkyhhho.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2usymlejy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ylocughe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2crqdwqav.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hhevuiuy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iexvtldn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2espydvwu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qczbkqmg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hpzdjiqd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2esheyrqp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xjgjqdts.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrrmyar.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwxdwdoa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rpwzbadb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lououxxs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xwegruqf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pskckjqs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hlxxgvrc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbrsdgm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2scnsvmwz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ifsdfezb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nuukjqxa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rftrpoda.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ootciewy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kezawcvs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2edpzghac.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kynhcmid.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbtiunq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwwwjrny.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nnzsdbev.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qgvxixsc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2easinuej.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwqyrzo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2donyhqep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kwubwzxz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wwviikjr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wjjqfjna.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pijemxis.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xsdmdzpk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2argjqikj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gnzlztwl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gomhzetw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lkyuumth.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mqtcwhnp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zmknjhsx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wevjdpsa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tgulxjzy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qwpnfzhv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xrbgngin.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vybouczr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tonzrymb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2riegoesz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kcbudieo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yrnscqtg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ozsgpbuc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vqqwowyv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ujwhogfa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dbbgvezl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jjldkbml.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qzjjcfjp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2liffvloi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dmeaivtf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hzmoafmc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dqyywsyg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zyfxaewj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2efbmlzxk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dgzxfmcv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arlrevrc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2solmimcg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wflaafci.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rlyadbdv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gtczcvnj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bqqkujvk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gjfveqvf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hxbzlytt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xdlqghkb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2njetrrea.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkyaccgg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhtmza.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ewaemndc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2myukqlhf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kzfgppgi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ifdymjhc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2onadflwf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jpttkxbo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zluybhql.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wjmvhgjr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2betyfchf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hmxdpsgu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2poboljrk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vjouigio.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pqldcwbt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kmbgymfo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ynzigdbc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ndppybqj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ockoyfxd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yebwmlas.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fslpmsjh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wlwvlifw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tvsbtelz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfqpysuk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wzdebeas.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cwahvpcm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dbygjrrq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kwmwaqaz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ephbctyu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2duntuols.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kduediju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2behieyzr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zkhrfjqf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2quzynzyg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aiwgwldk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2exvitzyz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mcomzhzs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cvuotixi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jzlozuom.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rpmawolt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2llupegby.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fobpfbve.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tuzzfvix.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zdbdwfxo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vruoingb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rvphoirl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rxhvyxoh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2orudlqik.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yzgojzqt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gimuhptb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nzgdexcr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fqhscvmb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hdalftmt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kzppatox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gwiomizp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wnpfhbjd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjgdsfvt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2oqlzwhcd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lilengwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hyicnzyt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wcbczldd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tsjcsbfc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mqgyzbru.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sbeycsct.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2stzpxsvu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2woyigjkh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kdazbijb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmttwslb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2anvgzyil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgdoqra.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oianpahw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2btbvblng.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jytpoaaa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ytgrlkrx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vttsedpo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2oaymwhwu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lkubbxem.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2sdrmcfrl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cetxpiph.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bycmzzmu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wiyzhsoi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gyrqensj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vtuscasr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2czyivtzq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zfswkbxc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bfmtkhlz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pnlguykf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2drknziet.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wkxgsrun.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2antgonxo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yyblmqlw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gptiroxm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fvnkvywn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xjxykchn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwqifom.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhmroirr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kiyeemwk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2znbwprsz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2orjlkrqz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uwsukssp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pehgsqir.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xhcxawnv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zdvrttwf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ytaypjln.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hvbvdywg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvuozdar.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtchhcn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbtzfmi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kiquwhgz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jbnuwzwm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbymmpfs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2njrvtcqk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ogaxqiza.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cepaytqo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nlkyvlqh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2moiqgomi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ljpdvrfh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nxpmnets.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uutnsokw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2emipqwnf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mxutmoit.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkautstt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sncjnsyq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwlehfu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2arxenpnn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yuhpztbv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tdqdgucz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jsazjhpc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2edhxcrmr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rgylaexj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2stwfmqyc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybleiqhw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gcrzslyk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bccavztf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tyafzffm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ppvpyemt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lkrvmwfs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ppapqhrg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cpbelrrh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xhklsxfi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pkgtdibm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zltcugza.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsxwugi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tdegbzde.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dnoybawp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eyyubwfb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyfgnzpc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywojyrve.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tvlgijtz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rhuvhhgb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2laggfznm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qklrxjpr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jntusvdh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2goiwwsbu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mhodpqjk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jjlxjmyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiijyrhl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fyxpojyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zigzzuiv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2myjmoece.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dacdidlm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2garirrum.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cqobyotj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nplstwwx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cxtrrxxd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hggkazef.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2iqjodyii.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2etwpkvub.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kqvufqtt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fdbhaqhe.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ezdzcncf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eyispdya.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vejtddck.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lblupolj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2swezmvej.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wxdykrje.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ekwjbrlw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aiqbcldg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rruppniz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bogfzvad.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pvbyetzs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mfuzbzhh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hlomxjju.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vmzcbmkm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yowssifj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2idgfeyaw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nnenegii.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fozmslkk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2icesrelf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bdhvcput.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vtqrixjs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2thdxfzkc.html


<!-- 参考信息 -->