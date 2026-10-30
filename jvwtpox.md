代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjvowgijw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glwsjfynq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gecmkaoox.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmmdkbmgc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxebebfyl.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gualisrmz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/ghlxlkwzj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gmoyvhtje.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/ghaynobmb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gzrmjoveq.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gacyzffbg.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/grqrurgoh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gwfdmtdef.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/ggsutfuip.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gxhkdziis.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gcjaxltgw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gojtkajns.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gqpurhhzi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gxnyvvqho.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gcxdfdawi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gcaumwdqp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gedzsrdez.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gogbvoimy.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gkksvxleh.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gatctrdks.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gbjsytgci.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gpaxwfeir.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ggwtscgza.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gifkjiswu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gpczyqbyw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gthfivexu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gwotlojhn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gxoemevud.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gqolsbjqe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gbrdldvry.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gciwpmywv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/georfbsqb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyqywmasb.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/ggcyuohkb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gaxoelsbx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gdkekqhmt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/grnpmihyx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gjtydqxje.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gikdkdheg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gvvgrxfve.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gpcmylcsj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gqfjeymbp.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/grveacpqc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/ghbuxgsxm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ganzucxbk.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gmmxbypgk.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gnywsjlbn.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gxhfxrsxy.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gafqncnhc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gklumvjnl.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gstvfbxso.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gygfkwwte.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gezwaapbj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gdcnkabon.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gjbqyqxdm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmwasrzcw.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gfungaohd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gegolsqnv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gahrbpezw.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gjyyzsmis.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gyrnamhbz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtaibrqcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gylfclypn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gxnygsmbh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gujrdyszo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/ggfqcejwf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/ghdnamgoe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gkgcqossz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gmpbsevij.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gogsvqoqi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gxpqdfzsv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gofcxbfaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gmrbviuxm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gvvgxtsal.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gurdtdnlk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/getzhfnyi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjbtnnmpp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvuronytu.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqxoozjjd.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gobfwerva.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/grxbgjxru.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gkaatzfsk.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/goqexghfd.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gqimarhgl.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gpododhjj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gavsqefwu.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gsyuofanz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gnlwwjsmb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gxpxcjdng.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfwngnm.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gtiyblnba.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkbfvisvb.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gdflqyolu.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/glejdwbbw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gbxbvvsjh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gazjcuebh.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/grpyrxzsu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gynrqdotn.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gllwjfoxv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gukgjbzwx.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gwycoospk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gopmnkrzt.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmfmcpxrg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/geaerlndg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbvwrkgsf.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gxmtocslq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gvqfdrjgn.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtbnydjzm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gnzwrcuql.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gwopupaux.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gnknuufhn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/grzcvisfj.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/glkjpjdjb.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gzvobkkjz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gbnclikdw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gefnjbzum.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gfpbidhdc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/ghisijenl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gvlkgjirt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gakzkoqia.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/goqynjexf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gdaazivus.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gceqximqs.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gngayvcge.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gpwoigjun.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/ggcljlpwl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gzlvgpkkq.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/guapfffmh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gafhaomfe.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gixathyjt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnekhfuou.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gryxosgwr.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gzaeocumd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gfazomemk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gklubnayk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gackmhlfk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gtavemhmf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gmorhamqv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwyrbalip.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gpucyftim.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gtcyfbbdm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/grmwelulh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/glqwsuhcz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gkqoiaeil.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gkhtfjsph.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gnghfcnls.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gfqgwknbk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gtjjcbpfi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gmviecbha.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfdhemxwu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gmovfnovy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gaittqxng.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtcjrhtnt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gupthwlve.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/glzysycrz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbxdmapqt.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/goxcddehd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/grcnhxtsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gypfhyeyf.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gxzyxjfxj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gzmdwcrho.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gikwaiqin.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxwkohvmr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/goiotgoej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/goqdugwfv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gfdxouvjt.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/geuwjslgl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsahwdfdi.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/grqwdgxyh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gevarzxip.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gmahzmkji.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsxrmywsv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gndoyogux.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/ghrgknjjc.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gyivvyvwe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/ggnwktoev.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gouoghaja.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gylzrplbi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grfaqwqua.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gwfdlxtis.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gwccxljxj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gdgutcnzn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gxoemftyf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/guuvgquhd.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gpfkbfyqo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gguthvvag.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/grtnzcmbq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gmrdasire.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/ggtgkkqgr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gmlsxbofb.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gknyblmlk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gweikvvky.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gvalhtewg.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gezxucolb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/ghokttbvc.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gwdmooeux.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gdvyouavt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gyzvhkwoz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gfsdmfuyd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjskqpxdj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gkdhfkgmv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gpydyoajg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gsodmkegg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gnsingutn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/goxvuqmcc.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/giarvcuxu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gcxxfweuc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gjwvrjeue.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ghdcjanbs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gwrztjvgk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gfpabekly.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gotnhhyzq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/guxdidngf.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gaicwyhqg.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/ggfkwyzsa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gvrywxqtz.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gyotmqbic.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/ggjusnbtd.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkodpsirm.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdekecxkz.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkzennpgg.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gxddibdvf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/grrqkrwsc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gdmhneqrn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gailwdtxg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ggkdaipyo.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gcbpkxlqp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/godyonjkb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gxvimnefj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gtsyoyttr.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gqpjiwijm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gmjclhtzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gloqdusfq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gwmmfcwuv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqaxbahb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gudzqeftb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gpmevevgd.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/goteombwo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gftgqhkcx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gvamrigxv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gkrzxtlff.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gyhpxjxkk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gzolzshtk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/grmqhdjjs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvfnsitun.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gcvgqugtl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/ghvzaxnmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gncgwmooh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gfuunzowa.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/geympoccy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gjapnfhoc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/glgjbjydy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gvracrpjv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gtsbqxccr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gqqrfdzmb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gngzrsdld.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gluqiicry.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/guhlpzzil.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gthahyfzo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/ghvtanzrc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gthonfdjl.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxeegfzkv.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjyfoquvx.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gruvkfvid.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gybhinsaz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gaurstish.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmpimqpzy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzslpdabs.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gfcozbidf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gztzjwqeq.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqyetykih.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gdniwhecu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/glxigihyf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ginnaoypg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gofvboenx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gwflhfkux.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gglxbodxk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gaaencyfq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpsrilpbd.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gfzcfhsqq.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gjtzuxmip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/goizugufj.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gitilgndx.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gwtgunofa.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/geghnjxsn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gpbcvmgiy.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gjoreembj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gkdnwbbsh.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmhpxexqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gyqchcstr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/giltvzond.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/guanctsnk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gbzoopabn.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gejioisxv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/giamwdhfr.sHtML


<!-- 参考信息 -->