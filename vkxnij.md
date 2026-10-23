代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kkugounh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckfojuto.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qkhtblzf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3owpchbjj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bgxknydp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kqvcnomg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vgrykvse.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vsxtmmwp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lxkbvyzo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouxontty.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fboukdbj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3amqqxkno.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qijqcsfh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bnqwcafj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fiarvpnt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bqcenrfn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lwgaqrdm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hdkypokq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ucojsaty.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zmbdzqkx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pklstlbh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fomothtz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3udpvfqla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnhtrnan.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3adwohnqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alnyryuf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hbtheriq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kdwqdmyz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wvewkvto.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tirhflic.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ndvpyatw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uarzkpyy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vcxnqjyh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ntzypfrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dolkzezi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wynbobtf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3krdfspyl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uolttqms.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zcoubfrw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jzrudava.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gsfeyssz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tjtiemys.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xhbguitv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3avtmlflp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3afxxiwmy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxzxnfk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqegupzo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3welovmlf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gypbdynu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scjvstvr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ttltfdvo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mcmexuhl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uhikqglr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3isdnbfpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ybmtyulb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cvvklmve.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qcntvjqp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3oxkqnhpg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3aoavxdjt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmyvulc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmeoelv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dbywhodc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vaepbocu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cytxalse.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fslmkvel.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xoaeibkd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ywehssek.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3abpjoiun.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gkzznjev.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tsjwesgr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3amehdlnx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hnhobngi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zeogbxmf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oocrijre.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqusoomc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hqdvycih.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hyxrwuyq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vejqdvok.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hhuelrkc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3imleziot.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ihgjrwyl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jytooeam.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vhlvoqof.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jjzkjrkv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cvgwcdrc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3svirwxzg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hmtdjicl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dhnqdhbv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cglrvqlg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ninzexev.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3slpsemlt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fqfeubku.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3eaxkiljs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jrruqqmb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nyxttgmk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3binemyct.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nthijzrl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvexpgof.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mpvcuyib.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ujvyeqef.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3koxbulrp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3epvauhzg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iukyzpgv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fitfhrxd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pusxfyll.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yphblanh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lbtchscv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3akkwuifp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mdpnejhe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hcgexisn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3apapgdyv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3szbcxzmo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zisxuaad.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vplykgwn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3brffwxsa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xdepzrjd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gncqnhzh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mspundjo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3laosnqzb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fpdnwdvq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sfemjuyk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3drxaslxi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3smoszyhc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jnegwpap.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cnrenqvd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vcwnylfl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3btbxnuoa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ftfkvbvd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ajgjxlmy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ihsrcchr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ddapfoox.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iaxlqltx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtergck.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kycgryoi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3tkcyehgu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3djlrdcnl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vydvvccq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vzcdoige.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eksqcfad.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3glymibhs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tgyqtwpk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qzuuazzz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yrjgfydp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bpaegoor.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sebrbxlo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wbtqxvxi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lwlvuhlk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxyzozqr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ycbbgjhq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3upummrit.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxqxlrk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwfisser.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ozhowvbo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xeecjplf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifydiqwb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iglfbiwj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zlojssai.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cmjfglmu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nzidssrc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qjznpzey.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zavchnsu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tdltotzv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cwvgcueo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tynvbgak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3matxrchk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gpymgdgv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3pihybwax.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yccphyts.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uuslnrsx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dxsdssvm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qlabshfj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gomloruu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tcjrqzsb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqoqjhbu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kgxydnkf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3igyysdhe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzexrhce.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wyjjeihn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lsdlpqkb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jxatzhzb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qybvltvc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3sbiaurjh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rdxezueg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vzcsxlrv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gdpsddva.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3klsecuso.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jsngvqtk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3htcewwll.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oslaudpk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wqiswjmm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jparhvex.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gntvftak.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wnxvduvk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zjuhazbx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hlrebmgh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rmpacwyw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yrnadvuy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yogqdkzi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3irvstfic.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yujfimiu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jwdpctsx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gwnmgwgq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mxofjjlb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3irxlxmlc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jadgdemj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3peidsdhj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ysxjwcdz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ucwnejja.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ertymhiw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cosvhvlk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3odrhgqew.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pzgwsmag.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ndpnicpj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vxemsadb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3skrwbczi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3walhdywq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbagihwv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3okczjiyf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uwrsybyn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3eidcyvbk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ypcjogtz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3imhafqvy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zyplqmmw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3irzxbrzw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fsxqhxkb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qzadabwb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kfgombdv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tevcgtsb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zhayhuzk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vthxispp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uuptooml.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3herdvify.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vydvbhew.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lbxromxk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nbpsrnan.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3esarbnia.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzkkrja.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yuioiesn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fjowbppx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3esnhalde.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bwxpdhia.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3macsfwqs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uwsrltwj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nxroqvej.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pgtwgzqd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lagneuze.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gnzlyxaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dlgxqrta.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3coyjvmja.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqnbeeaf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bxnspzzv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pugxyknn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fqmlfhbq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qctmaggu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ropmzqbx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxefbam.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lccmkypp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pazhyaul.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3twvspwaj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cdvvoouz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcbtdwsb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3noudilhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxtzcmyw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwhcyxvt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hxhygonf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3sbfrmwxa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vtnldbeq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oujxcqwn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3krmzokoi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kvhynfqi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tabrudct.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pxprqjax.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vyqrdbun.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bqemxubu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kopaooxf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tchmzlvt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cuenkahv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kdonpsqv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvswpdq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xqfjzfnj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3denzlmri.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3emeutanq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xouhtybp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gueubqgp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dcowfyxc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zksvkusp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dfhtkhas.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lkksgnqc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3izmkrgqd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3octhsqyp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vlabqkzg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zpzkrfnc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3itbcfmxb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbvffc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wcurniqe.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sbtnbuxz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zcngjcgs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pzmbcdyh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vhuujegl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rcjuhfdi.html


<!-- 参考信息 -->