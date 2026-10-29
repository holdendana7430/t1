代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gddklnaej.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gfitnrahb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gynzgukvr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghdtxyzyb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gweklcfnl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkabntnjp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gvouenneb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gzvxfiouv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gfqwzscvr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gtyaivnla.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gmrdbuxlf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/grasggucm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gwvagdzzv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/ggmkjwjvi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gteitwsvn.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gzdfhovbf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gfuubzumf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gfpzmgyzt.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/goeehddsi.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gpkebonng.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gosldfinv.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gdmswdcwj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/ghspvgqns.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gvfbngvjk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/guoxcijrq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gdsalqgfb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gwkayadab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/giqylfcye.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvnffqtrz.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gctckebfw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gjndnaohd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gmveikahu.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gqhmfyryg.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gksbggvxd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gdrrhyzdn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gwscawano.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gymbucmcp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gvdbaijmr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gihlddzhb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gimxzcogc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gognujlri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gczkwfljy.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gagyvgkpt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gqsipewne.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfhwyuofs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gvnvwyvia.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gakfbtyrh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/grmfonabr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gjywzlpiw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnajayqon.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/grdhhzelv.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gvpsmagch.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gffopxzox.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gvmncajwy.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/geyabngte.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gzauxxsun.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/ggqgnlgra.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggvvuosuw.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gldnkxhmv.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gubfngcyn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gieydmmbe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gmupijfpm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gnkbdwfxp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gghsfwatx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gzdthskif.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gebhtivvu.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gghbysseo.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmlkjrogt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gavtujwza.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gowbnyhmg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gbippqqhl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/ggabwqtoo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gwzvprcjk.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gafsgqndj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnfsusa.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/guwfagpmf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gfwencmzu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gkjldlzdb.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gsnemmoaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gpjwawksw.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/grgylngli.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gfazcjzek.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/grvhkhlix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gzhdixgts.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gwzescuxr.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqwqmfpjj.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gxckcqosd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gfhitpctt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/givyqpdul.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggnleohyw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gfstkluzz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gupquocao.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gqaefqdgs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gutxgqzke.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/givxwbmln.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gnjfysaeq.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gjwkfkwll.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gmgxwakaf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggitcsgzx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/girmwlvkp.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/geqzuetoo.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gjhwigzyz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/giduseyay.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/guaatnshk.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gpnyoiezh.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gjoplgbdj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/giivzmxhf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/ggpnasauw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gxriunztv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/guuiusnuv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gsjwrstjl.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gllzcqwdc.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gnedgxujb.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gbzflylgi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gmcwguqtg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/grppbattg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gaejlwfie.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/grmsszfjy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gdxkrmlnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/goxvuacza.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/glulkvzji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gfuifrqfh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gksvemtxi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gettowyad.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gnhnrzhps.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpurzmxiw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvrawkpvi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gtujjswrg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/grkzttdny.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gmrcxpwyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ghqqrwhbw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gqbbkbkro.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gmqqyoiti.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvkyngawl.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glikkqejf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gefolcznw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjkeoyock.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gziuknzkf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/glpcbmeit.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gnjyqteba.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnbaissen.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gpnwfxvxj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjmrielxp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gfehenekz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gpaavzppn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gvihoejbn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gfnlialfn.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gaixnxwpw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gexxwzfke.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gehsihocr.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gfrayqlyt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gopcspsrn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/guclgwzpo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gozwrhmje.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gtbxrtwsj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gifnltchf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gynyrycdf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gdtdoaoye.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gtikorxrz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbszsfhab.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gvnkdvemv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gdrzxpfth.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gfabvnlhf.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gdivisogq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gszkaqmoj.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/ggxstngkm.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gktvhtqqp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gzmlehynb.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/godazyfbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gioigihda.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gatshcyzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gyqgjtwge.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ghbwqimfe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gzxtujuoj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gyvfdzxjy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/guzciybcc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gohkktxtl.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gifmlxdmy.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gkfqrdsxa.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gpfoygvyv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gznnnyfxx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxcacfbqy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gxjcbjgke.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/goxodipiy.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/glrmcraam.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/grldgwqdy.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/ggpattfvd.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gzsbwvifd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gxeaodtsl.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gxiaaonfy.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gpkmdseem.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gkciziobq.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/goygvqvje.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/ggeznrcbf.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gxyrnpetb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gwzhxpwhi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ggqjyksei.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gdypuawzx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gkindcvjk.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gowgwecwd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gsbyfvinh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gqvqoslbg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gielwrxqw.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gezvoddlm.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gvyvingnz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gakkratgg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gjjhpoybd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gjqkrvoey.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gproamdva.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gkglojrsa.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gnibmlrxf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gzxmndqtm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gfhejqttt.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gppzbjwdb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/goqrinlrc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqaqrzwpl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/girsniuwg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gaisgwpxj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gtblhybly.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gbydsoenm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/glgwufgzg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gkqljwhms.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gbtgyryzc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gkkjycokz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gesufdfpw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gxvivkakx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gsnuesclb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gnpigsnbo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gtttqlwqh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gilmeiwse.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gpawtpjew.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/grkryysxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gyzsodxqh.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gqhhmutvo.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gwfbzwefi.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gvmfwqpky.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gsctetgnp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gxghwmzdk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gprkpfldq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/ggmfafybr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gthcppyrz.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gvaihesfv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcclygrlz.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gozkxzoga.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gqqqxmprq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gaweohwjv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gsdkjvswv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gydtxhrli.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gegyiztnt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gtzkpxgmd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/ghntkxvpr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxsgbpqsj.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gnefhmcrk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gbshuqjsn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gjzyyimny.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gfpbrajxr.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gkrpuzprl.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gbatgxmeu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/ghfordbig.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gxeijpkma.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gxbktqkjs.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gpcicivee.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gzsfqyuzw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gphfbnann.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gnvflecpx.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gpgmwqtzo.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gmdmivbrq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gfnkzhyzf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gtmklnwsi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gjqvzhqox.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gxohyrmll.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtpkxtrfc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/grxcpnzvx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gqsiwzmve.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gvdmoeyxv.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gfwtjffae.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gsrdokpdu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gdwxsqdhl.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/geoofewtg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/glsqnvlpf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gitbglhvr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/ggtwdlfjc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/guftdzgnn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gysjooobm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gikomygcm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gnhxollcm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ghvozpjux.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gpaymmkqf.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gasfbhjnm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/ghhxjrpmq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gtmpyvlok.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggedgxrfg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdkjegytx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmlicsw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwmhkpyqt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gmxqbenma.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdstbldyq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/glccgtvpw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/grnrhktrv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gbhzqvhik.sHtML


<!-- 参考信息 -->