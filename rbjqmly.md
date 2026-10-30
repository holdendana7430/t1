代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gopxfatut.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/glffctcua.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gebuljjcy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmxornnde.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gcxekprec.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gllpldkhp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gkhetzvbx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gncbkncpu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gmtmqawjb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gdztdgrjo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/grkebnhxb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gvejwldar.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gvdztvnen.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gowpmknei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ghtlbjqvu.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/grhbklstl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gscwxwbzm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/glhspszzn.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gtfzbunei.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gequwnnpn.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gvyyvcomi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gndksptpr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gyockhzot.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/ghejojwkj.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/glopohhcs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcrieyhtp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfeeperqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/glcmhaaay.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkuraaubr.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gyonirfqi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gmsvqunkm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/ggiqqvhue.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gjvuficso.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/giogxzcqn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gsytxivbg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/grbmjivsw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gckxsamhu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gzftxqvim.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggzuztqqz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gnhnhqgcj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gokkjsxnv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gxywtazim.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gizyfuczx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gzodmiite.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdlegccbn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gtbpugnoj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/grnudawjt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gqfsrrmdv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ggpjcwwyh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/giehruyho.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/geadgeqbq.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gbqhhderd.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gytvjjfzj.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gqambmjrm.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/glwdumflb.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gwkmutiow.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gmxhvidjg.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gwkumequj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gobczpftl.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gmtkuikha.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/ghiibuogh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gbutuzfjx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gdtkcstrr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjopmtrpe.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjnfedfcv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnzcbshnt.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gvdhwwutu.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gnjucrhwv.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/giqqnkjnu.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gjrbqdfzu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gsixbnokf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gjimzuukg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gaztydhlg.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gaemkxvkv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gagpxvgpa.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gzaawqiqp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbqojvhwz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/grysxssql.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/glauhhfbr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gvjemmomj.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/guxhorirq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/grltwbeld.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gphaocgwt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/geidvytkh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvssnzlug.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gorpwqrnq.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gopkgovwc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gundyxopy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gtrztvxyz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/giystvthd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gktgnadaz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/guphplcop.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gjyrouunf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/geszankya.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/geohnupcf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gsppwizvc.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/ghyqhbkvc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gkwfkpfil.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gsoxjygvh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gpiwtcmcn.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gnnhdxkhw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gsryzkoeb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gbkaolsll.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gbazejyat.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gcyplsdus.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gnjfylcrb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gkkfozifh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjokgjfrc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/giyzvweeg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gtrcwyzci.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gpdfailpm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqygvjfue.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/grncjydbr.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gopveordg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gafwqjugc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gjwxdxcoc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guvvlexxd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gmooutofi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/geryprzch.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gjwuadwgy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gyqcrslxh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gbutvsruc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkzprdgag.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gaxlzaccp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gxbwyppsm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxaguxxlw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpfcuiiqr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gpwmzvngq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gyoamrnnn.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gzladrrfc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjycrsglx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/guoziiylz.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gcgfdkcea.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/grdtrdloy.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gqonppovb.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gktsxwkkm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzufgaber.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gdcsmxivz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gmfknszwx.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gmmzcaivu.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gonrvqibr.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gxqataylq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gkatfrhjj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gznywjebv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gswfhhmgk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gohqchgjz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gikimelxd.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gubwobadc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/ggqtwflmw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/grlacsqpf.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gariqbxrb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyyeickwd.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gthzhurrf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gijyelpah.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbnalyvfh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/getdeshjp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/grylqiaek.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/geqmxaqbn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gucncragb.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gjadgqfhj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gcclugrox.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gefrbpphr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/ghqfzoozw.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gnkpttuqh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gzscdtkgo.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gwahojure.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gryisekut.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwnmraeew.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gaquwwqxz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gymrsyaqr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gbudgepum.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gsmvnzyax.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ghyrkpgto.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gyulodkwc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gplfarccv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxrdmhd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gengkdhmd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gbiecpvef.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gpyxpzrod.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gckgdryxx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gsqkmzonb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gvcsuewte.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gpvljrvxz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gotqamhmj.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/glsvueene.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gkyfowyxa.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/ghsggwfrb.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/ghjegusdg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gojagpucw.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/govedonmx.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvsspobek.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ggapbmduh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcdnxvbtq.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gqeyjmluw.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gsqtbcsox.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gntxzccfb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gofgmdprs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gpvzyabuy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gztcjppht.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gqrmmazcm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gronbwrnm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gtlkrohlo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gugjchmrz.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/glhweeqcr.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gwacwevhf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gxceziqrh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gnsglyypj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gufqzirlo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gpbdkdojl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/goqdrdvbo.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gcbyntzgs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gstftttqo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gncpqaapk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gcxfqtcnb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gyyibasjl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gjjldxvrk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdibcdzdo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzfbczhph.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gzjgnqqyj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gypqtkosp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gsnodyddf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gjkpwnsyp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gkzuwoess.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gbfcdpbkn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvuoistpq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/glcacuqkv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/golllrgvd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/ghsfdvvrd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gluchdfcs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gpqukbdbe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gejtcjzzy.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqayqabbc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gzjudmofy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/glaincgld.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ghfgrflbn.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpxxiuoiv.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gxccsgsjj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/ghemhbitr.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxvjirrgp.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/guravwcjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmmcdbroc.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gupzkqcfj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gplumplwx.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gtgrndmiu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gscupixgw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gmzsuflje.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/glkrzjjzq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjfpakyev.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gnbhngqpg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/geceydmpd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gcflnqtkq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzecizop.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gqzidhulg.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ghjgmifne.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/grwlttcfb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdswdtiei.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gyaolgnal.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gkiaamkpk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/glvcihaoi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gwvogdzsh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gxcckztjn.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gjoymrble.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gqeygzuxi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gyaemnaio.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmwumcegv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gzedivwem.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gqakovnjx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gryyuuuwd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gkubnqqwc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gabhclfrx.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gkdnhiegh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gqygpkuva.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gmonwgyhc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/geongwoqm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gjpzwutlx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmroauljt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/glnxprgii.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghmnkwfah.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/geoicauet.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gwyhknwqh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/goqekajjp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gjtcnajhi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gqurbewkb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gciiwxqjf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxtzrhdaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gqcpmmeji.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggofwlbfu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gnpozhode.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gnrbplrzf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gejgaesdx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxqtxxyok.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvmnbfkbp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpgdlderq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzvspscry.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/giqktbvqz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqmvmpuwu.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gohpvlnea.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gfmsuhdwb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gpwiizanb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/givafqiyr.sHtML


<!-- 参考信息 -->