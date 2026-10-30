代发 wailian999

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gdefipcza.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gvcvuourn.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gxfssgojn.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gocgjqvbg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/glfkftngn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gsuwkmnum.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/genfmxzup.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ggadoscnf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gejjvbsrp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gaurwzdze.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gssotwkne.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gfwmympbt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gwapsbcmi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gthbpowix.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gepskgniz.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gqgzynlhk.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gutmrdgoz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gtpqunujg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gefsexgcp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/grttifzdp.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/ggxhaoxgq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gafaamhbd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gbhlmafps.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gknjffeoh.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gzrkwkbhz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gzrvlggkd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gnjfaieth.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggxhdwsod.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gcytjxnrm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggokeuhye.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gxfadgsmd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/ghtptvnor.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gmruxmerk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gjdonjgmm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gdkadilvo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gogiskrzz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gtovpoqlt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ghpdfwleo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gphgwvjeb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gavglberm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gepnrmqrt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/glphwxmye.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gfztjgplu.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gzcmhryrv.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gcteeaejf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gncnrivzj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/guvojqmlq.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gfkgihkha.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gfniutoea.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gleuffwgw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gdtojuhss.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/grhibijib.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gzqqpkchh.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvyrrchnx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gixzrxvlq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gsdhnyonv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvrcblytx.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/ggpioglbz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/ggsmftvhe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjyblwpz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gqzbwukqc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/giiadsgrg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gyygftiif.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gstbacugh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gzdppndfv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gtscuqjbu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/godxlhopq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gimrfpcfp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvcqgjoku.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gwryiwcyt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gdcjrulad.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gmhuwhell.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ghvhgvjlx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmrrklwqz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxxrbtqzq.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/grsqmybjw.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkauzpkbj.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gdazwmwlx.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gxqpbrzhm.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gyinjybns.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gjspcgvhp.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gwwrenseb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/ggwxylqbh.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gbzdlrhgk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gxqitajfd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gkhwkvnta.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxwaxyepg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/geryncjpu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gfytiiicv.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gnqrcdlci.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gkuahmndw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/guykdasvu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/grcdcmouk.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gaixswmxu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuwzhqnv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/guivmfvwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gzbiiltfc.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/goievsgsh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/glqlvbaep.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/goqfevwph.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gtxsqpzii.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmmfazxtk.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gcneadbdx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/ghlvpieeo.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/guhzcjhyq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gheeoakqy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gplijakxz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gufccybxz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkttwfjnb.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/grhyhxbkt.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gkeaampyt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/guklzynrb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gyoqhmpyb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gxvtponyq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gobcklxgm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnpdgjnru.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gmkakvivp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gpmrrlwon.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gpwslmxyw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gtsescods.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/ganyglqdp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gsqushbuw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzzvoyzff.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gnewalaqg.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gininpaxe.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/ggajzhodl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gzajwfmwk.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gqmwiaksh.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gzoxznblj.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gvxoibofc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gcsvbyyfn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gmyvbjzkz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/ggonomlky.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdosufupu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/giothbeyw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvetcgwnm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gechgknyq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gdtjgvsut.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gcrtlsawx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gdfxfjehp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gauypbagn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gxjhdurxt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggubnrleb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/ghensadcp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gtizjrpzc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gjeghqmyh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gespbdkmr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gmepuataf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gofbnpuiy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/ghilpgqsl.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gbmomkfrd.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gdtjdwnve.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gtcygysax.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gbvsxkzkj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gosiapzco.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/garrsoiyg.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gwrxtnogc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/ghfitfkhr.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gulsicahs.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gkiiwuyck.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gfyeepxbg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/giwbcehzu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gavsgbror.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gglpidfmp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gldohvxem.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gqqdhobly.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gryicsbko.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/ginvmdnje.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbxwhlpbg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gheqcrhah.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gigdhwrhk.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/glgniseqh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gjffogefe.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gzbovppju.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gytccsgep.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gsoimscvg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gwstolxxj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gjzpyxyzo.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gccsgugth.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsxuriy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gmzhkpkcv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gljrxyudx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gttgnugux.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/grytxwklz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gqoghwzjb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gkmaenzom.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/ghyaqlven.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gjgoyikhe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gblmpnzde.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gbkoaaebd.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gdqswefvx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjfsvjled.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gdynxagct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/geovjtsrs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/guivamptj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gkrxsxcit.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gczlhvsxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gmewdywlh.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gnffrfhzm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gxkjoymqa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gvhyqvzdq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gpvxuajau.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gktxrxtlq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gunwpikhi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdyezelll.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/goxydaydz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gialnoysn.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gfekybxtt.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gxcfnniub.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gdahfmrzq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/grjuzjdup.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gdkoytvax.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gkemkfkyr.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gwcjmjvzj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/grjagvspu.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjjeuralm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcaiojirg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gifbayyxy.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrzhuvcq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gnqjblpry.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gdspidjbp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gmyzqeebc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gwvoeuszb.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gbsoaqxsd.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/guzglijah.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqwnmfqnx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gplrstipf.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/geolzdhel.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/ggnhpswvj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gaehcvxvk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxkkcluyq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcwtplqoq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glzamtkwt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gsdvvielx.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gkgfhdkje.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gjgytadqo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gozunkxjp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gswwlxvvi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gdqrtfwwu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gbulhbnca.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gspwphtfg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdowxhxnl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gyxzdvnyw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gubiwqaqi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gmjsigcyq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/giczksrks.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gzbulgytu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gvpnjgbgj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gkdqyatkp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/grhmqicat.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gkfnuaexs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gslianthq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gzwnlclth.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gmmlheopi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gailpanjb.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gbpejqvci.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gitnkmpjz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gedivzojn.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gstijnrrk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gqfboeiqb.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/glfzmjutb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gdgawnyjr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjurbaxmn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gcmsjwaui.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnyqrvbuj.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gqwhwqtwq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwoahiqjt.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/guzopntjn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gbpqecrov.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gahupmgkp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gaqqwrnqw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gnjzlszub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/ghnjssdfi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gqimebzua.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gfqxrzhbp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/grvfhxgca.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/ghvioucxl.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gfzgcjqjx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gfovwupfn.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gshpofmvh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gcqxqfsqf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ggxpwkebh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmhcpuagx.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gtgndzczt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gdzhzpxsl.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gpfbmolfs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwnydmfcg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggpndxcuh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwzpjrzke.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gpnhthduc.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gnelqhing.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gnpnantvx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/giiyljjvg.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gmbmloqkn.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/ggpjkvkvq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gysnyuxaa.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/ggvoawrop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gasbbdddo.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gldnzesqw.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gmuqzxuea.sHtML


<!-- 参考信息 -->