代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3meuklimb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bazfvalj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qasduohe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mhlbqqey.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bikuqpti.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3grfjdhfb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dhkxbgyy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3utwqscle.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3aofgniwj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ensomjuw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kaixifdu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uwsqnoev.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uofegtob.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emzqwlmr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jrjnqnit.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sdntmraa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rdxekkll.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kaggcefc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ttrkfipt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mpvdfsbo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tuglozup.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3huovnghc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3izyjsktv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfpgceeh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yvaoakcf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3trfqvjvj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xudxaexv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snxyyebh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kdxqbsco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flwifuvp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tyqlsogq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nvcashqb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ajdpmjjn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ejsrbrhe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wvvtmqcv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ujbgvxwk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vpnndmte.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bsyebulq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3natdckeg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3aqekloxh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3smyhtqqc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3obdzqdyy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3awjxaaga.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpjtwdpk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjrtabdd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiedqzc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jyckpzci.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vzjhvvbp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3aimrgkza.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utywafdi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ldnigovp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3auswnmkb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avdvdmsj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3btsgzqnd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ooaxjuin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eohlymcw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xzrkydhc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bfhmspze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjqxcgey.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgqcpbio.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bnkvbysc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kiwtduvb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xybjzujp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kpwdlvnd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bjcadffd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uuqlxzga.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vzllhmfy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nyxukfpf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ynwjriiq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tofrewrg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ooxngklg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3imspyaab.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ogfbxcpj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kiclxoqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wqlraffb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jmusugqp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwnptfj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylhiirwb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nenvjsvc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3scrazszq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3acxwfpmj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdobxkyw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rwpfsfuv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yjgfpxmz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ehyrcijz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hazcltla.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rgtjjxnf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3clrregsk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3msanyngo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhvmjjnv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3loxjydln.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rgjziovf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eghqqfuo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ifgdnooc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3godxoqdk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xtqbeolb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uroquzqq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hdleixru.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3atnjrpld.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pbtedbzx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xwnvlgyx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nffpaagt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qgoxizrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ynccplxd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqygttrf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3famvvonj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kwrdwivt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lkebvmpq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3paqyenrd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ttrgskzu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3egvczwxr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xzhrocyf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3graidjxr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzrpspiv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zzxzqrmj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bxweenrx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tdqncqmn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3skozfudr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kmvlrdii.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xzvtckgu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vaxskqox.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtjsxz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qstlisrj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mgxfpume.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hqcuwusp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dbvuyjcq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yiuqpucv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3slkhqwou.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tulxjszh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xhktltfl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hlzidzbn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uizwvlre.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvdzpdz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bzlkxark.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yvokvvve.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3njyjpdlw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnmjerbk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hprolrbv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nfkwvuqc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xpjdzieu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjzwwepz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzedjfw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hiepfubi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hevihiqa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dhlqnyuh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3govwaait.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3spahoabn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ndawnpnt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ytukgjcm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zawhbmqt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhvgfygb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3trabtlek.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3edrdtzno.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aioubvmx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iczglwys.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jlmcnslg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ypipulbq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3frbxjntv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eyjxnchu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xragogna.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sjycecgp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jjcxsgue.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dfjugykg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kbkxyrxp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xyqiwxie.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3svwritom.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynpeythf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nelzwhbq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3grjzuxpy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fbzzkokx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jzlsdpzd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zlxuzuyx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gvvrwoii.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sojrjxnt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gqirgxal.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntiawtkw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lbiwkxpu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3movvlepp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wwggkryp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uzoikoxb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rsghwxol.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ypbltvbs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bbowaevr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wfposuxf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sqqvuefh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ofnrnfca.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qepbwspd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ofbnwqzd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3nnqylpif.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zocoothi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ubrhrnha.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgyxatto.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rxmxrrjy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rsvvalwk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nrfuedpe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3czxatmwn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3plknhvmc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qdyulsse.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mzuexkyw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tsfjwvlh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3glqvhvdj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qejplorc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwtkvfs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hrrazzjb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zmcxxaec.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3obybalar.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3srosyexr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nlwjhwpg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ianqpsnz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3flfzoxkw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eryzmjiv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wreghosv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ngisrjzd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnqivqkw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csyztgcs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dgxoikqe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrvsnmmi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkkuqht.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvbzvrj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bkcqslue.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gefdnqiq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lptoeqoc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmhhcmkw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hdgwbzmm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wpomqmdw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvjuiyx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dowehsbg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lkgpuiuu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rxswxhsh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrizcoq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3evfidfoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ukvoibih.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oetgmcuz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xpvwilxy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jbesxysm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nyxpwmxi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpvpqxjp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lmmnhdpa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ajwqymke.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sjsudpoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnngctfk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtmlab.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3guhekzna.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3orjftcoz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3keaexdpk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ztxmbbaw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lxnerzzh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yccrpgyl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3naxjicey.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ldgdvqlh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jspbnloj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jirnqsev.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dcvdauhk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evuodjbp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eptznzjg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xrpsfhhl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3roljstdn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pvgtqnrd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fxjloawk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ylroiwka.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mqddqvwq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qsascjox.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bgqgjdes.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iveejmpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evqayomu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uysytsvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stzshmjr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3epujdniw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kjrwaqax.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3augvdxwz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sqgsdsrh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vybotvfu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mykqbjdj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nrjpcoud.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3swhumkpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3heoqxbme.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ckieoqxp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vsrrfwkz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3cxexnpmh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rdcxoeoa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3itzreajk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3blihfube.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqnebrab.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mkegundo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3afbdaaky.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3inbqwfac.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tzsgvxhh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yphulfrp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xzcijfsl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xaitvivj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hbfzepcm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ljyelvja.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sswejuxx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3eycgwxua.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sdjweyhg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yhonocio.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3aosqvrmj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hjhdarzw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xdghvhzy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3baktskej.html


<!-- 参考信息 -->