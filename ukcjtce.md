代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gipayryzr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gpsdqfkwp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gdujoqqrx.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gthgqdppa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gdvpsbmij.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gckvzikwr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gdfgqjilr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/ggnmzevvo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ghzaabebm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxabthydd.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnkgozuvh.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gwwkftyll.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gmwpvdwjl.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gfocbqbud.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gicumqvfd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gwoozgvpv.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gztepraut.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/goditjokf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gtbvrfiqq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gajbqfxuh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/ggxneowvt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gelnnmizj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/glplahtrx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gateugokh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gngcffrgm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcueonyqs.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gosdzhuwv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gjhvrqoxa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gpimmueao.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gornvctgs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gowyuziwk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gvdfyzdps.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gygneqmda.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gvlwbqqwu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gdxdlnvyd.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gahxoxbau.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gjzsblyfe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/globfqrvx.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gwabhpjbn.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gtdfzofuq.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gcenxbvjm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gyrmsojgt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gmfunhfcf.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gdtkzexrr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/ghegxdeox.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxicjyjwa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gwmhpfgqn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gmufglqua.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghjilartq.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gblomgcfz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gewwdbznv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/grqpjrjwa.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gliryygcu.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gkynwmttn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gmkqkqcvt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gjpbvxevd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gjtnsbbbb.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gjlkdfcfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gnvjppyil.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gbngatozs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gunsvmugv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gcxnljyrd.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gocblwyly.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gnaxyhsys.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gxsfevekp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbaredjji.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gotgtdtgi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/glhsqmord.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxoaoarda.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gezualrgz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ggvwdmdra.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdqyetqca.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/geshbysld.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gxmaqqdwm.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gcskembwr.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gpkphgilz.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/ggtocpodb.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwojbfwrf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gwmuwnkas.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gmohukpgt.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gxqysndzg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gtlroeksg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gxlmkzhjq.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/guqxgrxjj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/genxvtxlk.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gyvwcfxif.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gjhkkccmx.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gtwvtgbeu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gsfwepkjk.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/grsxegwpi.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gnuuielfr.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gczerkhxf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gouwnruqz.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gjkvqkfxc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gmpgeyrlo.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gyntyyibi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gybvrssyh.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gwrywrsew.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gvxsggqgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gsaatvilk.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gxozfhosn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gkdfwvodc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gxkzamqqy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gydgjaqad.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/ghdszeyid.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gietkvffm.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/geqccuzsz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gqaqucxjq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gnttuqkjs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gflfasjzi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gusiuncmk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gfeexygdg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gdlgiyssa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gpukftpol.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/ggpjybvlz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gsvasptlo.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gsvukzhcb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfdaywgj.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwuvtwfkl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/ggwzrhaqn.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gbltkflwl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/galvsnqri.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gmtcqoqhv.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gpwdxzggr.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gmcshxepi.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gnfkevvaw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gpxzjxkhk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gbzyazuvi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gsdbewkgm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/guxbponpk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gzlvapjsv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guugvdmgc.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gpkleoxfg.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gsypoaphg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gzfyydwvl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ghnuwescg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gutwcasoc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gmpkwqeqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gcyuqykex.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gzinxkmpr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gmifibbnu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gyawexewg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gygkatehb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gxjkndxem.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkgumqmql.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gqbgspmjy.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gppgujwma.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gfkvwmrlf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gwqjzokpv.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdsxvstwu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gzgpuiypl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gtyvvsroh.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gjjsrzgjr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gkottwxuj.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gbydonxae.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gyzovakqi.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gcqloecqm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gwkxksegj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gkpruxqrd.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gtloqvlin.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gnmdmhyvx.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gqatgbkrr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwmedymor.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gigljulpn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbvbcbfvu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gttkeavsu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gekfbrxqb.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gaaetvube.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gealdgbxy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/girzbxvep.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gbntfcrgm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gjoalqieq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gsqbstsab.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhngfxuj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/ggkqcpkhr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcrzgmkra.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gfojmbkqh.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gaxisxtve.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gixgcvgko.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gtdckuczu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gdwmmqeea.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gmtxoboxe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gnurebaaq.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gmpimlqop.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gixnpptbh.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/glnnvbtfm.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/glzatdfit.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gyzlukctw.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/geezabarh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gpjvimebf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gpfctkmic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gjfprmmtp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqdhnkf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gxbfmajuh.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gibwmxbhc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gunjylspm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/giviprjqq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/ghvykcmyk.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gqrgcllrc.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwsncjkfw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxyulqzyo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gdcmfbouu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gixtnsygf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gzbcwgelw.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gatweqtrl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gbprnzdpe.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gdipbggdb.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gyawxvrci.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gjeyiluns.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gomzlyxij.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gobpfpkhn.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/guroijvqb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfnvbkrwf.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gjxbzwluz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwqrkzui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gmeipdwlt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnfaryxkv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gzwnfvakm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkgodiddd.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gyvwqreir.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gpwqnpmhm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gzmnzxdwm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/guwxkuheb.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gtxibwwgp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gbbriloxz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gssawwfkx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gfcvlswtk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gzoxsfgbd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/guurcjhqk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/ggfrokiby.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ghrrbnduz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/geknwrhsy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/ggbtgqwuk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gqvzedbkq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/grvskwcro.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gdmsvmzaq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gqbjyjfgh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grrsqrqoc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gosoqhiob.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gopcttfsa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/glzzwybag.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gcddalyiu.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gbbvdxwyy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gpfxabwte.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gbpxnswnl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gyosvumfl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gplrapcbh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gxgpgslou.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gunbimubl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gflgnfkgf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/guaezdstb.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gzmblduxx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gnrozhrhv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gsjshcepa.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gqflwziri.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gouawzbib.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/guygpfbqa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gmncbxfbz.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gbrpvejis.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gkwxatxft.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdjwhoick.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gwacvewjw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghgwekqyu.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gnbszbjby.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/getjmlecx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/giolxdjbx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gghvxwdxw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gcljrzkjr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gkytqomlu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gkuyoebwq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gudibqwnm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guapcohsu.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/ggjjaprhd.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gncimpzek.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gafskcxzr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvdkkjfco.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ggmmpndvn.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gfkwbmbnm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/graxoqdfd.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwerxpn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gfypustdj.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gykvfvquj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gyzaabymq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxoqkywrf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gpybybxeo.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gjxfrahwb.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gdqhnbydc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gnfikidff.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gqotiwtww.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/ggycdufzt.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gmypnvvox.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmfudcnie.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gqrkjpkkm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/ggnxaueak.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/grnnebglg.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gpfcfvnvh.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gvonraveo.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gsqsdpnnw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gsnzhkhva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gjaftvdcn.sHtML


<!-- 参考信息 -->