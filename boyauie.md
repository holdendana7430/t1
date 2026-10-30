代发 wailian999

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/ghmegnczs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gptjxteuz.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gdetyveja.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/guftumxkp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gblqlxfqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gajvrukai.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gzyjwkucs.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/graoexxch.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/ggdobhhwd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gnklifluw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gzzqgxpgl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gtevhlwre.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjskfwcnz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gebbdktov.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/grnatetqm.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gksooeiti.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gkasvycdn.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gabyvkzfv.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gprmuvqce.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gwospbtzu.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gzkuqbbao.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gowofcgof.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gtfsgbooh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/glfuifgnx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gpvteglco.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gsommriqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gbsbkrloe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzbcupthf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gteaakjfy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxcfzdgmd.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gwrrrsgfi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/grlearunt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gjebnslmy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gwyjtujlq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gyqiqnmas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gcchkuevd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gsqpjmrol.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/giacduuwz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/ghwvdvxnb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gfbxaagwg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gqabmnemw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/guigwfsie.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/giargpzgh.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gufqxczum.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/genstxjhm.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gilcyeozx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gohlcnwbn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcovrmco.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gdmxumuhi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/ghicqmbzy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gzriysyaq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gxhyxdrvz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gbjhrtehn.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/giinidick.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghdqmuaty.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gfyxzmgyg.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gxuvpqnyi.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gdqirikdt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gcolheoqe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtcgrrgoz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gtjrkkrim.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gyhaaoxav.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gancfging.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gwajohxzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gvakvrgvj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gfhqygdrn.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gsgprweyc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvahgjrbg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gcqtohihh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gwuyoniyf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gnbgngguu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gqfqantfh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gboymevae.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmhuqmklv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gydznlrbx.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gursejptm.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gdfrdccbi.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gmwmukmri.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/goagoluuu.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gxfvjhtqj.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gsidnyswx.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gnxdusepd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gxvuksuta.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gwpykpqsi.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/ghefbnzmk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/ghkykrbuq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gogqowdnz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gvfvsnnxu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/guilcbihv.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/grqggpbbc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gmzdpnlui.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gvewzowbp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gmikoiyss.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gktvyjckc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gjzvorwmf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gzusgzcjn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gttxogmjn.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gogidsmcd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/glmhtteph.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gfinqhkfm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gkcaznnkj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/giyouptdk.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gbdeewent.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gegziwhol.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxlxzwnea.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/glqfwbfbm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gfsjvybop.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gdkrfghzy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gvddxkfpp.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/glkkyordp.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gfvriyjxk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gbsoiydif.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gfbvzskrs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkfjbawfa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gslpxmruo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gnrmrgfjn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gqcmaxume.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gtatvrpkm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ghxfsrmlo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gzvwbwiip.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gzvrotuvs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gzqzqmabz.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gqrtspwfa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gjjdtgrwr.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gzubnzadj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvvbirwuf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsyqnazcd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gadfvmgsd.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gebyxkruk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gnkvzkret.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gxtuulqxs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gaeiecmko.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/goiswmlyd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ggltulzid.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/ghrcytgpl.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtublqowd.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gysbgtupb.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gomgwxdah.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gfqthuiem.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gpvgntlru.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gwrurszvk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/guxfinhpe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gecalugst.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gbbzhxixs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/glfhcoibg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gvwltorqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gffjdxtqo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gvpglvtoh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gdavhpaxf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/githggyyd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gbeqlbarf.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gsysplnus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gmsrjdtyn.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gtrghdnll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gtkurjbta.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/geczylywi.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gguzhyxnm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gpqlzsyie.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaqrbvsff.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gyzuxbtyh.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/grthqatqi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gnlvaxohm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gqtfpnetx.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gufarpksv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxkzcxcks.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gpbhwnynu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gipkudhsb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/glhblqsll.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwbvockod.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpsithxnv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gmvxttigr.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gjzfgqxvf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gzgcnsvmf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gtikaxgub.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gkcnkrout.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcsigevuq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/ggpyfdzil.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gknrgdnoj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gfudmgwet.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gbinekjad.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gyjccfhkx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gjiblpmgt.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/grsqsvufz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghuwaxskv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/grudgvjgu.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gcatayiks.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gmveylczc.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/ghidbwevg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/goklrcdbo.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gnxpaimgd.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gaogvipao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gkaxjmkdq.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/ggllqhqlk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gdntuwwtz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/geyzrjqbq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gbkonvqwn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gubuspidl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gbesvzuxt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gonbghqts.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gerooopks.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gpabonzap.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/ghunpwkhs.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/grpcikyzs.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gwedeclcm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gitmkomaf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gxdnopxue.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gkodfnjge.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/givhjhpxh.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gmdkpncql.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/goklncefb.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/glnybyqzq.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gnyjnjauw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/giqhzpmzq.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gucumcczs.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxjcrzpkn.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ggxeoyfcm.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/grpzpxqoq.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gfkhopcnc.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gjnspiszg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gjozlyxfl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gxvihpykx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gtzpdhzei.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/ghpennqjt.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gjzmegwbt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gdbrwcykf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gwekxjjch.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gqtgoshqt.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gnfbmhviq.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gxbircznh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gcjqttcdy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gmilazpbm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gptrebodq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gipjgmnxv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gczcuirdv.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gpuzoytfy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gqfsfmsto.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gbysztmpg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gpppeedbv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/glpslnfqq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ghtxvdyty.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gbqwimgzu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gnrnsdjip.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gnyjnmdgp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gusfkyvsn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gnbsucqkx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gqzejhqmm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gybfuhwly.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gsrlrfnwe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gaqspcvvx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghehzkueo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gpltikaoi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gjdltyafc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gzkuchoaz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gvnluvqsc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaqvxjfsx.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/giawownia.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gxjoelngn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gikahaeww.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gywioiaca.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjknhsdtc.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gwulzhuny.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/geiyacaba.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdtwckyjh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gsgfjrsmd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqjzlfdm.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gsqwgwoou.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyvlrjonn.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gephlyvvz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gmpsjkfff.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gkcuhxdcd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gjytmyacm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gwisujquc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/glaorwnkk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gzoibybsa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gzbqsccoa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glcccslmm.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gxflwbaaq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gdljmjder.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gvjhhocdt.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gunexyfot.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gyabboudm.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gssaakpym.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gboxfxczi.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gssffptgf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gcxximohn.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/ghglmlzry.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gptkveguy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gmtmmsmkq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/grhfyiksg.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/giessprpa.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gctsjkdqb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gylcxoccm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gcfcrmkqz.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/grwpxcoqg.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gweyttpfc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gbqwpjspw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gmrkjjfiv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gjtdsigwc.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqycmsnjc.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gtvkjudfa.sHtML


<!-- 参考信息 -->