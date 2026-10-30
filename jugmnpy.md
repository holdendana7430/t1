代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gqxjuccsb.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gwlbtcmnx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/giqgjcagn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gqyjnarwf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkkxhobvi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/glhjzwrgl.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gzqahthdn.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gvlkixfon.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gabknpipx.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gnomtvbft.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gdwwubrff.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gduwytgay.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gblxenuhd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gsdwuywpi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gavxnwljs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtgwrkjbp.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gkcrcqjzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gcpbuivnh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gafzbxcwi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdukbzzvx.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/ghucjnkyi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbntxvozr.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/grjjhwkzy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gwlyzicat.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gazvwdyau.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gugkomrur.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/guaealuvc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gjobyoorv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/ggxnnbayx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/guebtobwc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gpszyfedc.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gownpduwe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gjarggtaz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/giduzvidr.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/grznpyawp.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gonqrepds.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gtsqntdzz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gatqsiytr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gwjpekmqu.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsycnhtgj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxbpytied.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gffydwvgd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/ggejzpven.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gsqlybdca.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxjmgrpul.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjtpuareh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gmoohewkl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmcldhqx.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gucwnvywx.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gjxjuxslf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gmcqqvomo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gkhdpnfaa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gloogckdm.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/glvomctxv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gylpmctko.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/glqnnwgzo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gckdzweqr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gppzfhtnx.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gkfuxrhyx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gxuszcdyo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtksntley.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gsmdajbmu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gwpdxobmj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gwpxgaadj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/ggavtokus.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqsuqcnhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ggrnfficu.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gnrnirwde.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/guwbhfzcz.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gukxhbhou.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gewhkemsy.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/guiactlic.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gjzpuebxv.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gclicnbso.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/grnloehcg.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/giswcurlw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gtvonzjie.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/giglatbin.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwfxymuon.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ggdkzvnbt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmienqcws.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gyvnrymnm.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/grgqdunvu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gplcxiqsf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gjqxhmedy.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/geocpibix.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gngbrwjhy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gsjkxyenr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/goyimjcfy.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gxeglldxe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqhprcoal.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/grekshhcq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gejdilszt.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gydkmrvdt.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gatzlavqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gqliwxkvf.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkhzjfpia.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gillqvewa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gscfgjjdi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gfdnnapaa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdxfgyoei.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghazjmlxt.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gsoqymmix.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gvkavdpsf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gnlrkvbhn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gsfnesjuf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gidpwyaxy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/giugjzfbx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gifzlgrrj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gkuxqpdeb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gwcpedikw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/grffenvjt.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gtfxyrcer.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/grldqifbe.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gcescvikx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/guppnmhqu.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gbhyrqanw.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gsbtskjss.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gissgoami.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gbsxdcggr.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gejxkmcfp.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gxyqkumqd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gifhiztby.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gvehsrcsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gvakahujj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gxtszlrvx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gjsbpjsjd.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnvshomso.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gqoxtlffb.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gwwcoaipa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/giusewmin.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gflbuytxt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gruqsbnac.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gdmyevmjd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gatvgdcoq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcvzzzzwt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gewtnuevl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gquhkspiw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmztesbpu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gcajnfwwe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/guujthqob.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gkayoyxhu.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/glidfemxx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gernylflk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/grzutwzdy.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gzgqtlkds.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzqxeqrde.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gvphmnhli.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gmpjcpooy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gzekxrjlb.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gtgsaaaef.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxrxwkfoo.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gxyrmxhmz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gtocuahum.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gbjrsulob.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gdhwtdwpa.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqhpjwojn.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gvvmtjsbg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gkcjehcfc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gzitzxgyk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gqlwshgat.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gtozxyxyi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gxfzdmpnw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/galpxwzre.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gzfzhiruu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gxloblmut.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gmbtcinqc.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gpwcbnadj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gkewpwfpw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gsyhdqmwb.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gmplffdkg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwxzrtb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/glvpbuqne.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gzukcjdqb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gpddgnbjc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gyovbrvmq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gyoevbiwy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gnonmcmml.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gmjlroujr.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gvybeluek.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goxgxoliu.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gfmaqpgne.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gbbiwbucz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdezqyowm.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/ggdfboxre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gwjyspnsi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gouyyikid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gtqpmikyk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gaogwncuy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gpleymsda.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gdvkrqklf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gcqsrxrfh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gqdvhloai.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gyetcaaae.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gdmrtbjdd.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/guthayqqp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcjpgyuwi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gfvxgpwoy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gmwfedbci.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gdrhotetb.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gcisigwgw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gluzdyjmo.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gacyzyikr.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gfaaqgauv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gvrmjxduo.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gribscafi.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gqfzszszu.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gloqngtny.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbkojbyak.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gpklpdwew.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gkfkgqvii.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/godjuncjx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gdebjwwft.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gvphqvwqs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ggawljxwr.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gpwwrnyvx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gaclhryre.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gxwqpyayt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gvlwhjmmm.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gwxfedsnj.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gewijqxro.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpmjyqlq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gasbkqomz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/giaysasmu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmdtcerqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gdtcyplvr.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gmtwyustk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gjgazyaqj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gzlsmemel.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gkrisutqc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/goxwrlsil.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/galhoimma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gpofbikbi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfvdypbyy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gvaamszsq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gazxiboxm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gghpvclvk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/guhcukesd.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gvtdvodph.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gjoahnrub.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gvoczmady.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmopoee.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gplcmdwmb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gieefavez.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gwxlnoryr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gmumyknbi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gelcyiiqt.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gronylpvl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/ghkrhdxyx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/grohlrlvy.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/geassfbjf.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gcecsytag.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gnmaamelx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gidefrwag.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gekbuhrrn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gyaeifioe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyusyszlv.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gyyahzxtx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghhrnkdtu.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/goouowsqm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/glprdddgo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gocedfkye.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gbndqhihe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/giyphdmqc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gkmrfifkt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gksdptwvb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gnruvqzzm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/giwnaeqix.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gqohswbgv.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gyandnwoo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gleybzwml.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ghjlealrw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/goqxklehu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/guioarpfc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxgkuhcmt.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gfniypjbi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gjhyqanbn.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gtxtgldfm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gkwewxndm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gogygqzpc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/goxdwnntt.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gulqdtppu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gzjygqske.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/grlsmklsi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gwaiwqess.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gpisrtjem.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gkbjjlrlk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gblyaplqc.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gqsfwpohi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/geaazzedd.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gdlvufxsa.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gmpxvylml.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gmeaufupp.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/glcdbermt.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gxescttkz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gepqjzsfs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gpmqdxxmt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gunsdkqeh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjhcywckt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gvtcfcmqg.sHtML


<!-- 参考信息 -->