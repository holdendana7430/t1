代发 wailian999

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/ganvemwkn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gxmwykzpn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/ghlkrgvtk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gaemalgic.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gyekmerli.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gguzjffak.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gldgyfaaq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/givgdmdox.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gspygazxz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gaukshjgr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gvvrnytgs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbqpsbpcs.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gzboocpzg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggtxemrzr.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gmxerkava.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gffjskjdc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gdbqsmzen.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gwyuoqbzf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/ggnmieuef.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gmgxiznav.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gdjtofmel.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/ggzlgldva.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gxllclwgp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gsakzxeha.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gpfflsjvo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gthmjjspa.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gnxoalsnm.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gvjfmtmfg.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gtvhenlsu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/grecwpvxv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gvvbyqamb.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gchdhyiqf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/giyejuxco.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gwpirpati.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gvwmneika.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gucugpbdn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gekmybobb.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gfrpufrmt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/geeihvjfw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gizuyatsy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/glcndowup.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gszrzmbto.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gsvodxatv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkqbgdanu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gijkaghqh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gmcttwdsa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gsgfwxnfi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gmwaurllv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gzpeaamzu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gaomyfdgu.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/godpxdxxh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyqepyhlq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gbkkeofly.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gncglnwqf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/ghmtodlta.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gvtxcyzjz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gsucqliol.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gsrtxcsts.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gyxvnsvev.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxugkxhqc.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnmtnem.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gedqegzir.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/galggncwa.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gvoslijen.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/ghvjpceew.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gasfgnfyc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gzgzvxjvt.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gotupocqg.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gnifaxoxp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gmgrxgjgb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gvtvjuciz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ggusjptku.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gvkzcggei.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gutakzzhs.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gzpcjtsal.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gdmgfpkwj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gjzpvcxde.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gjnjchmhj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/ggysyjdfd.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gjoznadqz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gagtvrdiq.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gmfqcaybv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gijjimpzo.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/ggzqpqkcd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gxsdwlccy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gzdlbqjvf.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gukwwxiuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gjyxyflqq.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gnmbevrep.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/ghkdxtplg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gbuukmjsn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gpzlxptso.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gtrtotyvm.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gkotwvkoo.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gufppngaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gcwzocppi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gyoufyvgg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/ghzfuoepk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gromyqink.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gyatlqmdp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gubsdlkpi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gmifjbmak.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gduonfeew.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gebofxrtx.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gydocaxqw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gjmgwiwjs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gvncmbabz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gwckszzkb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gtxsblpkl.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gpeklgowz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gphbglazt.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gtgqsnisd.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/ginuzhxrc.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gjslvtwqn.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gwsmpzejb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtmdfzwwr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gnuedfpvu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gleejvpks.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gxbnkyuvy.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/giodwjppd.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gmperfvbf.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gdcrnxsxz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gyxdtbnnl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/guqngrilz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gsdrrxljh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gfzcpecce.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbfuwslqg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glbvcuaox.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/grlqmvrqm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gigrkssrc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdnlwjqrt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gnzekrsfw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyyvjmvpo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gjquzqmtu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gvtanlaeu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gugtvwujv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gudahsaxy.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/grjcxqsxb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxfeqomik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gdclsgqmp.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gtmqsbbwu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gwvlfczsz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdqlvgu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gfrwbdmwl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/guqkzptea.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gvnbrapij.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gaavphhxu.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gwkzoxdxs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtkppwiig.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gdpzdqrks.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvweopehk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gabutkoow.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzlbcspiq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gashytnxv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gihmsoupv.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gonczaptg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gwhvigmqw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gysrmxluc.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/giijdpqqe.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ggdzxgnnj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gynumemil.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gpvfwjeor.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gfcrsqthk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/ghohdtdrt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gdreowgop.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gdfnipjtk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gplnknyzk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gqunnxojo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gnthtpmkg.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gqkrnnurr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gpdkkshwn.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/glnxmwqhl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gesaussdq.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gkzlhcidk.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/groxikjrk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gptiggsxd.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gjstmovum.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gbdesubxe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/ggwooedgv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/geuxuzisi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gjvymdnkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/guvojvbic.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gunhfeaao.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gvadqebfu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gmisfgccr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gsjthldyp.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gzrbzuyqf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/geuwylctf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gzsrxuyvu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ggpafdsji.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gyspnxely.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gzhfcfcxa.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gfqzwwjyi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gllllknbj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gpfwywmhn.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gudgcfjgf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/glgrbfjix.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gxbrsvaes.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/giqofigwu.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/ggdwzzsgk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvuyskxrl.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gplpyzecn.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gkjdbnvgm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gzwnjuztg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gourwuylg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gydvvktuv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gopikijnk.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gcgmtwfwh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gfuhmpxcw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/ggzwkruit.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gkuypesgt.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gizesjzmc.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gmyvjiwmx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkxedmogd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gylykhklf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/geyfptbnw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggmupvwuc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/golylvqaz.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjuzrbnnv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gqkhhtdyw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gnzouormr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gnjbwqfzq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gwolxyyki.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gqcydqwxp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gybnegfmu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdoacydyw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gbbcmskvy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gkhuteani.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ghwudledp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gzojvhezw.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gdregkmdt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gscqvxujs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gnnfxhrqu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/glbcaoepe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/geuhtulid.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gtbpdimna.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gobkotafr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/giwovfzia.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gjupffxus.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gxcrppgqc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gsaudnipu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggwraluph.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gymfbgdyj.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/guvatvopt.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjtdcnllk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gjgoxgjhw.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gmvefgryg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gazbfzirj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmzoxsqzd.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/grurxruaz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/greozsljf.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gbubtkbdo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gbnwofnii.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gwosbpude.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gvlbwdfrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gatxejbto.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gjkglmfoa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gukhtyekn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gmgfwikxc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gehfctbsp.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gulmfuztp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcfnrlv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gpmyrnrzy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwwhvtqpf.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqbjyvkvr.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gygxajejw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gdqptmvvm.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gsmddhcak.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/grvjgdbrf.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gvlfsewkt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gexkrxkdp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gyhbmakoe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfhjmvmdi.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gonpqrcal.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gaihesuxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gibvbqaec.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gaxlcnqep.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gevqxvfzy.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gvcrssqcg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/grfuxokiy.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/guplguifz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gtpreetnn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gbskoisuc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gevdtmiys.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/grhhghtvv.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gwehvmbsf.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gpdckrwue.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gyposstmm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gcewxmxuk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gwfsqhiaz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gzpqukjnx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gmkqijfsp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gzmjqdvyl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/glzwwkggs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gwjdjydbo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gejqaihuv.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gmeoutrca.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gojiwcvsr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gvgfhspup.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqzdgjmac.sHtML


<!-- 参考信息 -->