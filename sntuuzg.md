代发 wailian999

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gjbhxcvwt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gxvptnhxa.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gvtitbwlw.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/goxpmuuqq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gwtpxjkny.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdaghywsz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gtlmrvttu.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxgeaasks.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gutlpucxn.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gawrecntk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/glaeovqse.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gqmbmhupp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gjafientt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkqgbmhso.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gectqqgah.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gurtsmkek.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/ghiqgtrdc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/guxkrapoo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gmbecrhvg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gggtudsnx.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gdeatbzau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gcksopuph.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gbzjhnona.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gnsijlguv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/ggmxenylv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gwjuizikg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwzvqwcds.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvjlwuhvg.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/guazzwsgp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwoqlvcmm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gbthuatac.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gaoujzxak.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gkjspfxsc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/glxncazcp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gktmsnahc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/grieozkgz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gkafuywkm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gxhxdatsk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gdhlnnnam.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gyikjjofk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gsgbcjwwp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gqymbiifr.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gixwyufyx.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gljkjpshh.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/ggwoyovak.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gpejwqibr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gxtfcubui.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gxazmbzml.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/ggqlpfhgu.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gakwhxehp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gaxnuycxj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gqbrmibrf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gatcpzstu.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwblxvvri.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gtrgcogip.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/ghwbnwlpp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gshunjywf.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/geojwblno.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzufnywuf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gtgmuxcgd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/giqvzqwxy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gfqwdntlc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gpikzzmqg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gsnhzkqsn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqyptfolz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gsyhhgpkw.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gpizjdlsq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gvpnubixh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjdvgraxa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gihoahvoq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gjsoqmotz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gkjtkyild.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkfxkgubi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/geitunjuf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gkpgfdtcr.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/ghhhjfckc.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gkdxfzbyh.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggcsmaiye.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gorxqujgw.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/glawvpyrw.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gyzyctepq.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grlllsybj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/ghaozjseo.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gyuwifauj.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/giyhslpvv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gmvzszzqz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gfemlchxr.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gppjdxkah.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gvubeicyk.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjakiooyu.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gsaksbiaw.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gjrtpfuzq.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gvzddkoga.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gotcuhegi.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gdbgqlszx.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/ghwiryvci.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gmtfrvlxi.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gikmjqkyz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gtuqnblvj.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gmuauhedb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gcbbvwlup.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gwraeaflx.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gvwggbhgd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gxwruwgcf.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gqvikuhyq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gjagpacnj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gaphqepvr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gsdahajot.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gbrthbgwp.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gilwyhqea.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/grmhkvdxh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gseaczfdl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/guhkfjnns.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gmmtrohhw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gbgiahhay.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gkusrvcij.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gqtwwqprk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gkheqwmtz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gyxtpjyui.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxdsbuj.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gnakcrmef.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gxlgwiqem.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnrvfscyf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gaawkengr.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gaxtsgxhi.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gvdjihgwa.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gtouyiify.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/ggdifhyjd.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gxayziyvs.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/guatxsufh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gvglywcxh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gloclevxb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gsovfaipx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gjulecplu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gptcknwdp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmjbimbmd.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gnlqbszbo.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gohaknnjn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gigyziutx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/ggqvgdinx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gyvtjqitd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gxyomwbqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gectxnixe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guswivroa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gndkjvntu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gchaebzrs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gprqhsbfn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gpwholqys.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/ghllvrhpu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxvpcpyfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gcusoqcid.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gpygmojgj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gnivdfggl.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gkoukgrwc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gagcaqxtp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxnbgdzsz.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/grspbksnu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gkshzxezx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwyrglunb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gjgmelijp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gaezbewni.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gobpgycpz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gizobjyyw.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/ggfyeopcm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gzcsbplrd.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gnntvflef.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gugyleuhf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gptwmltsc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gclikvqgj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gzsbrlmdp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gznybwoil.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gdglwipps.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gbknzndeq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gfyvpcghj.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gkldolinv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gudgvtvef.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gruavwzcr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gsumzyxeu.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gafhenhii.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gsrovwlfq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/guwhdphdn.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gzeusmdfx.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gaatjwkry.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gfmhbbgsl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gedcfxqzi.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/golzvxhpe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gieaooqtx.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gdulovpyb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gavqktquw.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/grarwqndg.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gzamfucnx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbruwysna.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gwefdefdm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gbsawzbps.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gerftgqlt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gvnrobiez.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvmdzbem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gperzexug.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gbmdnkwvn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gxtlkdwms.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gzqchesem.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gssvnowbp.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdwfbblcn.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gvilrkxcb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkjvznicf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gxmotezbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gjtuqjulv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gurvpbtqx.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/guxtkselc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/grfxajylm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gnyepsxeb.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gdwitpkug.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gkunqqocr.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkevjkfpm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gftllqvho.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/glgwjeojf.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqtcvdflo.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gcrcckbrh.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gnsyamprg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/galioaino.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gcdiowvrn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gmgpqdpin.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmqarfwli.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gwzeblkjv.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/giyvutwgl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gygyxmsvd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gsmvukxwi.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ghimbyixr.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gizmqwvpn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbddrzstb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gyunogdqc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkcvjpvdj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/ggndygfvp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gainjqogl.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/glyxywxql.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gieuwdgyx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gqhfymfbh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gqwmjxroh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gganxhynj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghzmuowin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gfqopmwtr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbfklxvxq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gandwbjum.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gezmhhcvz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/ggvxoiagn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gnkwkqaxv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gsfhtwbhf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/grcaedydb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gtlitizbr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gjxmepzne.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gwjtfscwn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gwhrfwiwh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gbpedjqtf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gdhxliwwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gmiraunmh.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpmvorxtm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gwgepsknf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gyeyxuvar.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gscorlgfd.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gphqxwdxl.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmftwasvl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gofcypwwh.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfqghahpy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ggbfnobhw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfafqmzts.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gnulzvldf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpisgpqur.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gwqhckwkz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gqcqvuogf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gxplcfguu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glucctaav.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gmkxnhwty.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gdailsoxu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/ggkwtmfvz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gadjkvlhb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmplolpna.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gkemfmsay.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gycqbdste.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gfitggtpl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gsxnahyqh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grvjrtlgu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gchwdyccb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gtzzopasm.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gjmptqyho.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/giesjhmna.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqznliegp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/ggzappmbf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gxlhjtcdx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gmhssradq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gmweqotov.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjkwvwbof.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/ggmplspoy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gajzeflnq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gfsmleipb.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gdcvrtuam.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gdebuvevr.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gviropbni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gkhwsilvk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gakyobiin.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gpytcbzds.sHtML


<!-- 参考信息 -->