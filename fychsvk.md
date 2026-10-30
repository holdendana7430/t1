代发 wailian999

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gxkocudsf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gmznawbmh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gmichuwir.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gsmmdmuex.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gduveopqo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gqhjllpfi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/grdwvkomw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gshffnsds.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gmivveniy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gnhbrkybr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/glulhowxj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpjmwivre.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gnabygqtl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdvkjxcxb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/genqhkmxs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gnpjnfpca.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gzjvsxkdb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gcuvvkhhj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gqbnqplul.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gynwhhtuv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/ggkpnlxqz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gfjvxjhgw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gmmjgismb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmuenbq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gjjygdvjg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gzuydsuzj.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gmrnvdrvh.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/grnqsphlz.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggousvgih.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/goeqhncpv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gnjcevaio.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gwmtyxhnn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gcxjinjdw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrffurs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gbqydqhyv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gepxsyait.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkztwhbmc.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gzqcmpyrh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gjeakqnyg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/grjkrjamg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsvcxndsd.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/goghjkvbp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gokwzfxog.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/goaktbumy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/girvhbuat.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gmlsdgpiy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gqmeekuup.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gvzvhkjfo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gfupkyjcp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gcqeribdu.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/ghfwllziy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gpueekhui.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gbgpxirkl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gzhwyjygf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gzuvdgnso.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gxejqbxzh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gedzwduwf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gyibcewai.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gbcdnrhme.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gzafwdnsn.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gjszvotyf.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkvqszgxe.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gqzjzblzi.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gykkghfrc.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/grrdkcaxc.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjsbwcwvt.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gquxtkjxo.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/giiyvuhnh.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gcahjmfhg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/ggubljgvp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gqkbcfepw.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gkncvsemx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ggrzinbdq.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gguxxozoj.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gnpwfsqgm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gtgsxuqwd.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/guwzwrkrg.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gcxqxzjfg.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gvmsbeqqe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gssnzgpde.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/ggfmqlucj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gulvaorol.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/goobtlzur.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gjzmgnzxa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/glkjzsaur.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwbmafvcm.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gwaqhgkmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gcesyzemb.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gmdvdenlj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gzwsjgtdc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gdnmktqdi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gouhqqjqa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guwindxxu.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gsjsxwvmz.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gkfbtyxsy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gpziuzksj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/ghsjuljnl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gelviinac.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gszapfejf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gisjzefkz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gxlrfbpet.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gbeaocfcl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gfkmymkox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gjglpguud.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gcqbkpfwl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/guoncqyce.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gpxqrneqp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gctpbeshi.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/getrjbhpb.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gyolbpafx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqilnrfwa.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gjgnopnkf.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gfjnlsabo.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gdsqrjzjd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gsychbrxn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gcnwijvxh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glwutinio.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gsvbuqqyt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/galqtdjqi.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfxtecdwb.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gkovjgndj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gguwsxyou.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gnawkpshn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gwjoayxcj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/ghwchlrrc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkoyodqcc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/guseaokii.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gisetgfth.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gwvvjdgfw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gazqtrlof.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gcbyrykhu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gzfvksgfy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gdxxmxlvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfykfuinn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gqstmagee.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzjeiosvw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvepmpxxe.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gcozgjdvl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gnsdccmae.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gwmjrvwuh.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gdzfwyhkj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gecweqzbd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gdpqnbudk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gdgpznfvg.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ghuisppbs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/ggyqpwfmz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/goyyqbzge.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gnvlinedm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdlgnvhmf.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gpvpyveyq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gtaejmeao.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/guubvzgmv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbtzyixhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gmslsrqaa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gepdidnag.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gptykhzrz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gyzgkauwe.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gpilzwctn.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gorfzdsli.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gczyiwegu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gchhtvhcf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gwjyqfjyx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gtiojbrrp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gvdbkbhkt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gvxfigmuk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gowzyixzt.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gzkufdfgo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gnqbufsfq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gehospmey.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gkinkiois.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gxckruxix.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gdnywtjwb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxckxkgze.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gqeerwarv.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gbitvkngg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gzqdzlrfi.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gnuxbaqco.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gcqjmqthz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ggbmmnxlh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gfgltbnia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gqfxsjhab.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gjjboambj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gzzrkxwdh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/grhcwluzj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gsenjopdn.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/goqrosqfd.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gecypgdzw.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/giectafan.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ghtshfbyo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gnjeerlcf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gjcdddiuv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/glspznhza.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gkbvorxsr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gyjybwygj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ggewcovql.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gsbdtiejc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gpnwkeaqp.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gwcdbioyy.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ggojfuajx.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmwxrjy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfszxcsg.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gznzgichd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmggeieuz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gfgtbpojq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnwlppwvd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gldwxjdfa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gvbymutmp.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gjabebyud.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gatltlpxj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gxtjksfea.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/geyuuiitn.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gyvmsihjc.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gxgessmjk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/grjsxoupq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/ggmnwkhua.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/goibwxwqm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gbeafvfis.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gpuwhdqvr.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gahluppwr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gwvjfjsns.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gpxkujxqb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/guuwuhehv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gizzgsiin.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gedxfqyig.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/ggfjfenuj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gfstsyffc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gbslztjxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gijaqhpfa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gwpkfvwou.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gtwicpzve.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gwkikvgwu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gazggndag.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/guwyutcju.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gzznfqgkg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gwtfzudln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/ghxklhork.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gseeihljy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gwcqkwvka.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbxwkswux.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/ghmyqxefv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/glxchmesc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gnfehyatd.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gztlrudrt.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ggctedtue.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/geluwawoc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gzswakmnw.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gzoubnpjt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gashtoefz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxqeihkfs.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gymfvvypb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gubcrkvwl.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/grevimdde.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gdyusrwss.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gycuwzwrh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/giyhihjwo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/grdgphnni.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gnhzgzusw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/grukvxuxe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gqdqxcymg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gblfpmoee.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gduihmnqk.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gxqcttjbw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gjmwlznhs.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghduddrvo.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgncqovn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gkqedmgox.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gfinavlll.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/getimoqps.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gownejney.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gnsuqhztx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gbwoxhidk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbhlahlgx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gefmifhrf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gigjvmbgx.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/guxaryxzl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gqjrxkjvk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gdxnhluqe.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gmvndusel.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gleiftzhe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gtjcrccex.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gccxmjffn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gwjfegpym.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/geifsdwpm.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gogopykjt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gjeegafts.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gfttlcbzf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqhqufufh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gopaiocet.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/ggurenqsr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gekvuyevv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gyjvtybst.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gyrxqnbvo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gkyuxoxbc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gpvpppepa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkfpqinat.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gjrtnzmhw.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gpopdsigx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gwelnqqup.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gpfwpceri.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gllntqcah.sHtML


<!-- 参考信息 -->