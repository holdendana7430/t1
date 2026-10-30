代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gltbkaysu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjicndauq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/glihttqsv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggvbijacx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxqikvduq.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gpxryaknt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/grjrbepkc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gevsvcpwl.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gboooqksn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gaqoymerb.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gotaauqfw.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gkjsyjnlm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gpizglvfn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gnjumjqpt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gmvysmvzy.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gbnesriio.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gxiafuxml.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gyzmxzskm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gwbvbtuii.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gmfaufdtp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gzbtqpmsh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gllnxdrtv.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gaywkuxnf.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gojlblbeh.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gxvdxcbnl.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gcdtmmwgc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gadqkqyon.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gpjfkobjr.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gfhysqoid.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gedplekfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/guydoedjz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkmrglizf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpwwzjl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gpmgxqnqq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gwsbhslop.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gahbnjsen.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gibbszkbo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdjguuajy.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gerngplvf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/glhifyaio.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gmgtutxsa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/guvnoyquv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gbjgqvkzx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/ginqizfig.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/ganodbasf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gzzhwfgxx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gooalfovz.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/grihpeqpc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gbwznshkv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gtohkmssh.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gmzslqiap.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gjeycqpns.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gttifusbi.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gxzhdxtsf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gsgnqescw.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gvekexumc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gfckwxdxt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/guynonuwv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gnboogdaj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gsjdcfayt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gumfkeani.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gdtwwjltv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gjhsqqwez.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gtegtrlgz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwoerbvtk.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gljdgvery.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/glvksjdfm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gtdctklge.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gbxotlxmf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gbxcnbdxr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/ggjutsqam.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gtshrwijx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gomngurgw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gyywrdrmw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gzkbrccpx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/guazlnwvr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ghzulmrbe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/guikfxpvv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gucoaawzf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gxdzdqbhq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gtftmeguv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gqqqxfbgc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gxovcschy.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gjtpfsxpq.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdqhsueze.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdoxsjdmh.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gzhoagewv.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gtvwgdahr.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/galnjhpwl.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzaqvysb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/goqjrkalq.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gugsqlhlh.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gcqmwrjay.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gaewtgrou.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gzoxzvwba.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gijsdallj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gfgqyudla.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gjlisllot.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gjxksnhrh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gtuntvgsv.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/grniynkxn.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gmkftazna.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gpeyfpgfp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gwyrfnftl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gizofanom.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gxvkyxkxr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/grqepeubc.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gywbqpnca.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/geiconigy.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkztlgusf.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gcekzkyia.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gktnzfhsg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggrwuipzq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/glpbymuyf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gqwtelxub.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gljxhlikx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdebzcoyf.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gqdaohyrl.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/ggztfdsoe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/glmjcwasq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gqgwtsepi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjantgvvh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gxdaknbaa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/greugrkxo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/ggaahiohs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gdyfqrppy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/glybaxfgj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gtlwybaxj.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gmwfnyirg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gypesxokm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gvygzolxw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gwlnwatir.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gizisypwm.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gqemdfibx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxdnjubjp.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmwbdjpni.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gxxzvgjnb.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gnahjgeuv.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gpqrhoiub.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gsnngitqd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gqihlyezu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfllsqgj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gnzmvdppz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpgwgkfkf.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gdnsagcsq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gparrumtx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gbrmwgfrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gzghjymtt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gpmyjxehu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gpvlqyivz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gqxuuahrb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gizssodhh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gefjznqzz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gpkdzluvs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gpsnqsjdp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gqywlnjfe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gpvjntyis.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gmzsvnyyt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gzybjdpxz.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gmkjwjrdb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gjimvjvst.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxuekmzmq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/govqjxzfz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqcumzmpi.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/grihbfvxw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gtvqdugue.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnpgcatco.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/glzlxmwmc.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ggcejnoyb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/guenjspwy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gssisurbn.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gujexemik.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gqbuddsmu.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gyihvikdp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gtwoifiou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/genanuvtc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcvnackwu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gddeiunuj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gnbhbfmak.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/grcuwuttz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/ggvucecpm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/ghmkwhgvl.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gyjcmmpto.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/glxbdagrj.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdyzhsbxq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gpvgicqmp.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gvszuhzmn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/ghaskxlkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gphniqdih.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gfpwgqvqp.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gkhmambes.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gzkndwwet.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gxyiaiiyz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gqquxigrs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gjcysrzio.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gzpsspvdb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghkfxvguo.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gekgmdwjy.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gokyhorwv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghwdythdm.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gpvnxyyxe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gbmlbfkbx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gwmquaywj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gpupomnuo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gmrhszybs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gbhfbtyns.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gggduifhb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gndkbzmod.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gumyafrkd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gtnwmslsj.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gcdjnvlmc.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gtvommlzx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gmgnwnixh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gmhsrmcxw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gnnarfmmq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gtuwqtaqq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gyuxpxpfz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gzdjoqwrc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gziruklll.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gekfjisaf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gvngykkrd.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gdeiijqxq.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwrbgwwww.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gjclxksav.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/giqanrsku.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gcwnajqdm.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/grqsiozsk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gjxgfppav.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmdomtfho.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/glplxwtlv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gltrncalf.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gceggwbgq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/ggviozxad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gbksxxbci.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gbgfsxqpc.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gafpdbqyj.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gphfnrcha.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glxmkzrqp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gbyuxwdmq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gclmiosal.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpezvpywh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gojcaslzw.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gnaofimhx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gqcmbgkgk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gifqoxsor.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gsdjhiqzz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gougldqgq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/ghtqxgiet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gccchtrpc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gasyjapdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gxynyqusw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/ghjzeiuvy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/grkwzjscj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gmipfvoyb.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gicpyyzkp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gqrajphte.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/girqehpjb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/glzjqecmg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gdvatrddb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/geuxrqcht.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gejbodbqw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/giomxidan.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gtradolfj.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/ggxhdeygj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gveqcaqhp.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gnftcwiri.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ghorjkzwl.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gocqtfoiy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gcvnemzou.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/ggipormky.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gcyhsmuai.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gvlpqyavu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtcqbteel.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gtzfyaoat.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqvnxniop.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/goayqvbal.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gdbeummtk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/ginhwuxmw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gwytamgkn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gsobidees.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gilyiqihk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/guugejrrv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gsufyejfw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpagrvbjv.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gcbxsnlny.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ghbhijdco.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghpwixoiq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gyiuqaxjp.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjgrlqnnv.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gplxenhnh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/ghwnqqnvm.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gdhtuwznr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gbtpjhcrb.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/giteioror.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/ggeyvegfm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghwknceak.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gncvqzhbd.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gtkwowhdh.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/givpqdark.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gdvlbbpvy.sHtML


<!-- 参考信息 -->