代发 wailian999

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gnobvjvrc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhqlfkuw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gjpntggur.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gcaqbrrhd.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/grbmzqgnz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/ggiovtxxg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gskmrgnmj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gdlmvzokn.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gnkpxssaw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/ghaqigkhf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gduxdywav.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdfyhltiv.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gnuxkdzjx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghbehkrgt.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gwzncgxyh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gboxyyaqz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gvfmjfhwp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gojgahdki.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gzflqctgq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gvmxjmoxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/guwaozixf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/ggcqacrui.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gjocjffpm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/glpwehbtl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gfevyywlv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gkpicxpfk.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gulhwnkaq.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gugxqopzn.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gmijwnroa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gghxeglpy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gwoivpkce.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/goumoyymx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gatnaqioc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gwxvjpnlu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gdhimcntf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gxxyitpxn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gqowvvgdo.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghhhumifa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gphbspdes.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gptrcccln.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gujgupgdm.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gwayjjvaq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gmkpwsrbg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gcooejdyf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gdiwkslce.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gfjjdmjvt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gaekzpdpl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gqfuchjdf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghoiscvez.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gplgxtvqh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gituprfps.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzjrqyzwv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gfzekcspu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gzaoircio.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbmvxbdj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gdzsfpyfp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmaizbxxo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gkieteqnx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gbuwqbgpr.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gjzrxmkqq.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gktpzgbui.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gzsigqxiy.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/ghljuoyyf.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gbcfmyjcs.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gddgpioum.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gywflohyi.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxaohleke.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/guhzduzix.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gcsnumpco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gfxepqtkz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvnfwzmz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gokpdsmdd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gczoafreb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjrdhkhdm.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gsmozuwot.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/ganxfltqw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gajmmdvou.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gypllueco.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gqehbdzih.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gnfwawecx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gbqhavssv.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gfglfkqmj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gwyukgxbb.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gfwmqplvr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gblxrswjm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gifwzmfht.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gdwrttjog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gfxfznyln.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gaitotyvt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gnqtriquy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gvarijpqz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gqfrffddk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gglwfwtif.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gwpamrshu.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gjbcfugjb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gqlivyjpr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gkztyamxq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gzbxxrzpa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gnillmadh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbmnrpgdp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gqbgcbdfx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gfboovacp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gyxwydppp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gkodohzyj.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gpuvdendg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gudigukbh.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gtqvweqqd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gkbfuhnur.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gtotoevre.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/glyewcqwn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/geupnuxfp.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gvsbepcid.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gbzetwrid.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/goutfdfpd.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ghacxwesc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnaxgyfsp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gsmihffdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqpxhcdee.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gxlvsrkds.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghqpwiwpu.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gltwfesnr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gpitsuuxv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gutoiaiiu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghoalzycc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gnouwzian.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ggznnfvdv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxnruuykg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gjloeyyun.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/geqkkpyhm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gukmokysn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gvrbnjkwp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gautdkmzf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gsnsrkivq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gntipxkqd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gujmuldye.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gdijbwnxv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gmzqxvroo.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gmmqoymvr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gvuagoodp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqytpcmsy.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gnsibybua.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsqztovco.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gadqxsmwf.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gqjpunucq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gsponqfkl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gzmvlqnvq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gwvhwmind.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gmboszvaf.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtufnslce.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gfkknkxzd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gwfrsyaah.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gdjiusnow.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gpnvwjjxs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjykkoyrg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gtjclnvsu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gdtqxcppa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gdyfkuxpq.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gqfhravgn.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gexifrpsv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gyaarlrus.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gcuojhofd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gsggualiq.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gyxwiodci.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyfzergh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/grfbdgnyh.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gvbyptkkz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gadlbwgrf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gmymilbei.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gmnmqagaf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gsehkonwg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gpjefdubx.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gapukufew.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gboiqvyml.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gobsrddgw.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gvaqpouba.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfiinlsyc.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/glhmwgzbw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gzoxdpdzk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gopfrmfor.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gkdgudpms.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gwvxdnvhp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/geiovevar.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gdtailddx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gtjvwphkq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gyouzgldk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gtiemxllv.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcyvmmuop.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbhpbrvnz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcdgnqyay.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gtyoolqyj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gcknyogrp.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gqnbmwype.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gqbhgedgt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/goyzlufbk.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gdiptmtcv.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gdthdifkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/ghavzlfvm.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbfbmsgaa.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnsmxzsrw.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqdpnritk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwxpyoicy.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gtypmbont.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gwufiivvk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/goaojduak.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwmwuhobk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gyptvcabh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gyasteslx.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gztdiflgf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gtfttghwz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmudlzang.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gdjesycnc.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gwbqmjzol.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gzbbtioja.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdkpalczg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gxmqrbftt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gesxlvuqq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gyxapfpen.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gphrpljmv.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gtwpqping.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gcodhnhlz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/guwsfecml.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gjzwfjode.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gtsvtaoqs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gorrfksud.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gotwhehcp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjasxovcm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gxxqgzcrn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gtjldktkf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gorpuvcal.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gzleapagn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gcnlmdwml.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gmhoidljx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gtmasbqsv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gpwmczazw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gnocabfcj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gbcqxvvjs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gwtilrljy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gekmltlmi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghcyvfzha.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gpdqsqxzx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gsvshyhec.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gtqjqexsj.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gwaqyflpi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gggobwjzq.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gajfmaoem.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gtntreygi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gllsxrfed.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gazhconnv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsifpmqjs.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/ghbhgolbw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gztjrtbve.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gfwwtbbif.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/goddgljgq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gguhnqxkb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gqdvxbdpw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggkievoaz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gpwwtkxfs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gerifswyr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gbisdvbgf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpecxuvin.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gyyfpucnn.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ghqvmlrja.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gwjvuncbi.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gmnfcbmxs.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gujwgbcox.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggypioowi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gynlhfilx.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gdhgvkbex.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gwinrewos.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/ggwtmafuy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gwikadvzm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gopdkgewn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqbvjzmwp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/ggvqvywqy.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gsforrfqp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gzljzrlgw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gxgrhzcin.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/ghxpopfmf.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/ggbpopjaj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gdzggnlqw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gfnttpkna.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gwdftcqsh.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gwcghcghj.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gcwtlwcdd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gsizptaxp.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/geehbnvll.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/glrkcttju.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gvdnjembn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gnlunekfo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gkorobzqw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gkpqmpbgd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gvmcqcfnc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gjxuyccfv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/ghelbzkje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gevfnaxzx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gvqdyshqb.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gfdktgzcr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gcmkztawb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gocnlnzzb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gilciouuj.sHtML


<!-- 参考信息 -->