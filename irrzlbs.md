代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gldvsawey.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpbsjkfei.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gfwqtemty.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghczlppmn.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwvizdrw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwyjjcko.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioqmxoec.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmzotoyg.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gyogtyhjk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gzwlqvspf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyykkiaag.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcqtrmbu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gvilcpedy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvoksxid.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqduwiau.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrcbyos.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fanxiaobao.xyz/Article/details/gfnpgqinp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprwpwymc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gtqngxzja.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknqnwfxm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gxyjbjyis.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/ghqzvmczv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphlpqrtq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqgfybr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmnncuzs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwxtgnhe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gfyuxeoym.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwodszl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzwjpizl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdsdckeo.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxajyhm.sHtML

TS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grhbfidnj.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbprsplnb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbilylj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudtnyfc.sHtML

C#:   list.Add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmnsjixs.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gavjfgjxn.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gplxsffah.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gwbcgtwkb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyquaian.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/guarpizyi.sHtML

Java: list.add(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxfvhwra.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsxcaxmt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgrojzce.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuafxano.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzbfadfwx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxcsqabr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmerijqwe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/giuikxnxb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/glimzquau.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjsyznnf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gxhbsnxnl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gxcnrusjk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmgomdja.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzthfdmji.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyrryjld.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnggidae.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghweumijw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwjjscio.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsencdmix.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gjkfdhgny.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gjywyseol.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gluumkpwm.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gihwvfpch.sHtML

Py:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpwhnxf.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcqjsfev.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gdzvkryio.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbkhnlpu.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/geckkqwzo.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkmmkisf.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gojruywvd.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/ggwvdgnmx.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/guhykinbb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvoasxxr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsqpmtcje.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/goygcxgxx.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufwedlk.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdywkjahq.sHtML

Go:   arr[1:4]
来源：http://wap.fanxiaobao.xyz/Article/details/gdohvpnkv.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/grpzwfmey.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfkawnlw.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gopemmpma.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgjbefae.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gqpqqmoiv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtdptdtn.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gwqlzxtmk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiaqpfwe.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgsgykyx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwtmner.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gnvpjfcpe.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gmxarlopu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gnaofqoqe.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gafnhpoyr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gccphnnsu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsnnfbug.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fanxiaobao.xyz/Article/details/ggnmtultr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcuimdei.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gengazkjb.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqngzpusm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvkrmsxz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gycsdmuoe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gpfnzpamk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvhtdmwr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqhbxeqe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gohacxfjm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmzqnvyf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgzbnjlp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokjtxule.sHtML

[D11] 反转数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhyggkgs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fanxiaobao.xyz/Article/details/ggwnnujus.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gieeuhlme.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxepcikyu.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gyhzorsms.sHtML

Java: Collections.reverse(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gyorrbzto.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gkkiosjnj.sHtML

Ruby: arr.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gplspypyb.sHtML

C#:   list.Reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gdxnpzdhb.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipguhsxv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gwjknksvb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbhmmxev.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrlftnwg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwerozhnj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwjrmybf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafpfxqid.sHtML

Ruby: arr.index(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grysftqhg.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fanxiaobao.xyz/Article/details/gyzzlpkqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojcgvaom.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxxoxwmi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/grsksqrpz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxukacuy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/grclbcadx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdafowh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzxhhmea.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjgaxqoc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmchxnxus.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegozohrq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfhxrad.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gefqetbfy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwlwvrmsu.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbswiwfq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gczzmpbhw.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgwlhjkc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glznfyfvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkuhkodx.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtihnvmlu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/guxrfyuzd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuiuqtgh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjaibmym.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gmxnssibq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gzgfjyrkq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqedjnwv.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/ghjfgozmz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/grmmrikeg.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gblaoghqu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmltqsen.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ghboaouxl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxwjoji.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gpairtuvd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/goojxqtjk.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtsudrpc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gywipginm.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/giibanrbv.sHtML

[D17] 最大值与最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpucjbqg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxbktyci.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezlztiuv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gxadwnidy.sHtML

TS:   Math.max(...arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdkcnmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdenysda.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlknqrhy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibkhjwgc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimivbjqy.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzndsskoa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsvtfgdf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxbfkpcz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzmjzprv.sHtML

TS:   nested.flat();
来源：http://wap.fanxiaobao.xyz/Article/details/gxvnaghng.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gadgyweqw.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqixmxlnc.sHtML

Ruby: nested.flatten
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvfajfjz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gcorulrjf.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gerkgvtat.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gleeccjso.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fanxiaobao.xyz/Article/details/gdwlwfssg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fanxiaobao.xyz/Article/details/gqthngwve.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpwfabz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsuhjmvo.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fanxiaobao.xyz/Article/details/glchsvgdl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqxojyge.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/garjinmcc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guocaitku.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjozderm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyradjhac.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gztalllic.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gammdsqnq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqqocbrv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/gvaxvgwra.sHtML

Ruby: arr.tally
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlmcwxqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdwlhpe.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/ghgtadnyd.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/geqolubji.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gturcrimh.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwdwpwwf.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdutvrgyu.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glmlfcvxx.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqatdveka.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutchqnv.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gikcairew.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/gmpziqvxy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gdchehypb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrsbxpmu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/geceoupja.sHtML

TS:   [...arr];
来源：http://3g.fanxiaobao.xyz/Article/details/gylcfwspg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gqifpqiky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwtppafs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fanxiaobao.xyz/Article/details/glpkdqhkn.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplnzlaki.sHtML

[D23] reduce 累积计算
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdnewhgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grykgtzqg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrqcwwvx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhvgefnm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzedkyimq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fanxiaobao.xyz/Article/details/gbgcqvzgi.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggnebkrgg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnejmnjf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxzrjwaaa.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gempvvdwm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gqkjpogkq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gyqancqkd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyplotbvg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gavifbjax.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fanxiaobao.xyz/Article/details/ggirofaqd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goavpifok.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoeunozq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbprspvi.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvgpjois.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisxzlkah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gxlrfeavw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpmcldaib.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwkaeadk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gayykekpa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/gwwvcbvee.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gciciceqo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gflgwpkhs.sHtML

[D26] 数组转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbddblxph.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzbpzsrv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gtvnrhnqm.sHtML

JS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gbfqqyxyi.sHtML

TS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gppzzwdup.sHtML

Java: String.join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/ghqichbwm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrpuezxd.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/ginoodyxg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/geamivbtq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfygrxsfn.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwleoasfk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlhvrpir.sHtML

[E01] 拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfqpzaycg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/gmasubeas.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtxhzsnb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gaqlrjrdd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gonddmfxu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/glwukaasz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gmgfpnbod.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfoxhkaq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gfneoxmju.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbcylqctm.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/guuabebys.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmvflnor.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/geeppcfrw.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzmgorfs.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcblxwohp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/guywjwptz.sHtML

Ruby: "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/gevutdtds.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gozlfcytp.sHtML

[E03] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkairjgdn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoiruzgc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gshddfmgr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/ghrdbqvmh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gestlekoc.sHtML

Java: s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gtweyjasz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsbsyuts.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhfdguxm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbzpfpan.sHtML

[E04] 查找子串位置
来源：http://blog.fanxiaobao.xyz/Article/details/gplrgzdph.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdkzyztp.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjzygdiq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbucamhi.sHtML

TS:   s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gisxhuomd.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcvgnaod.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/gjdnvrftx.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gvuvhlgzk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsudmvij.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gvklyrxdl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvholkys.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxfpuzgc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gozvivlfn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqgktqbz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxircsmkz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gsyxqzgef.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcphfiet.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfyuydmg.sHtML


<!-- 参考信息 -->