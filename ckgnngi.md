代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gvxweqqpf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/grgxblfdc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gnmcpttjr.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/glbvhdngz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/grclqxklf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gnlspbveg.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gtmxdmjer.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gnqhtvbim.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gvzdelivp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/giafmbuyy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gscxtloen.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gngmazchp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/ghkzfoqkx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxehgmedf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gjcssrfjs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gehfhtgqf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gzeyfqlfr.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/grptrtxul.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gpanwqymb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gnnpxymcl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmdoxusnj.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gcqauhezl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gduqqznwe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/ghdcjpcea.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gefszyjxy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gvzliehxh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfynqylcv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gdgacckqy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gvlivpydb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gncjdgyjq.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gzrkntfcu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gnwweufan.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gvakjzevh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxcvtkewu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gbldpjzqn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gkygupebo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmalywwyo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxkbwvqbd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gqihbokue.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gmpcwmnoo.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfktdpsmf.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzkxrvkag.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gphspthdm.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gfpmboacp.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gcryugfwx.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ghjfswyfz.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gpggldhaz.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gthtzjsqu.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gdodnifmw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gtzrkhsbk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gjvvskdce.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gljmypkff.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxjeoqbcs.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjsvituga.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gebqjjzbd.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ggtoamoog.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gevbokplo.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gvpspjexs.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/grofohbpv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/galsmdkws.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gbomjrzcl.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gesivjiyi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gmirzxddt.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gsclvxcjz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/grxzmqcuc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/govvnfiqy.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gmcqgkryc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/goiyatekk.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/grxfcnojh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gxbvprotp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gtfxsktrf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gqwqxptyy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gkdbqrzfi.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gpainilvu.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gutxfwedx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gbdnijnqk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gxduyaoyy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/garoodzge.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gpcsciwmv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gjclpsbcp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gzxstdedd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gcyfpheoi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gsjpzrapl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gqdnoejtc.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gauivgtcq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gtdwkkrlj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfqhhtplx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/guoxcybjx.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gqspzxdde.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gjajjbptn.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gdlrnrsyb.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gzkynbcov.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gqinvcjrv.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gdclofxeb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gyceyqudj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gcsksawqg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvrtmoclh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gothmyutc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gquuurlzk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzkboosss.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/ggyhljecz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gkmlsexcb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gxthfmmyk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/geggxlkyq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkppmuq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/givbarcam.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gercytzxf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gkpxuixpd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gsbqgiqea.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/glgnpnzkq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gdiiyaiin.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gpgdkwjlv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gvjtmoebj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gqaeikeml.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gakrvqvxg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/grjixqepe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gayhupqqg.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gailvozis.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gspyxgngu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gtjrxrzkv.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/grbexjnft.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbjztucon.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmcvprqfv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gzfwgveow.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdrzdvonk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/ghxrrjxvy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gyixeyrig.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gsdflsdjq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gzoroigdy.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/guctkctfl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gohifabme.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gnzbgxwjr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/guvgmwnvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdgjeipgj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gigjvznoq.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/goituvgwi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gkobqzvwh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gfhemdpme.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gbynbmond.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gafsigmuv.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gumzgsipf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gramdohnb.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsydcshmg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gvbbjeghg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/ggsxzmmqg.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gzdemlwmb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gefcblgsv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gvwnppote.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gkqofczsv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gbjxpnbrj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gzvreithq.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gzmfrelff.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guhptjsgs.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gmxtqtrqx.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gyiqldokv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggpexdksk.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gmtvwewjz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/grsuwohwy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gjsrajchf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gwmgvcbnt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfckeormi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/givcdxpmr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gpilowmxc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gnhzfrxup.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gjefhxrpx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gfacncngo.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gybdrkmhh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gxwkxwspy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gwtbvplth.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gvbnlrwxd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gchkzedib.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gpnaderyf.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/ggfnhdqen.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gpzjfihyf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gvjhvxnjf.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/giixoazxc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gtrxuhptp.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gusetltug.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gduabroeq.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsquhcoaq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvisveqwl.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gljbgnuja.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gdzxzocev.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/ggpqcwift.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpxjgxkvv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gvpekrudc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gmdckhfks.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gipsgpxfd.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/ggpsfbqmv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/glwofdcnd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/grfqbqdja.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gbbiaurbr.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gfkqkwebd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gkrtdtafz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/giqygfmkx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gxczeplfo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gtompvtdw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gwepohbfv.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gnfcfgvnu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gkalcxtzz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gbtxdicit.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gqjxigjee.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gzlerucip.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gytvzcabu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gznbiflyr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gjkrviotc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gfmtfckns.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gwnugucjo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gegnyhshx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gvhxwwlcu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gcwcvmnja.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gwvcklqcp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gunttnifn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gcubusufe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gzljjcvum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gufxqtdwh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gjagitfcu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gbpugxdvm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gbabyoyge.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghoztsizk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gagfnstjk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gacoszmxy.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gigscipgd.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gyevhwvia.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gwgmgrvry.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkgtheffl.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ghdotrnus.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/guzrzalap.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggxttpmhx.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gwhoghxvi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwzzosvmv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsdsgvzdk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/geuxeftta.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gxpeqlxvd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/geybymgjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/ghdpqqdda.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gdtdbtsiv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gznutacts.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gemcxgljw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsfgppwsx.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcvbrdxjd.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gjzfjuwri.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gntewsvqy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gbhdgortr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gdxpzuerj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/glffyracl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gakdygryw.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gnmdlgwnu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/grikcpknu.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gzbfwqeay.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/guctxhykt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gefvenwze.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggrqwyrlp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gpcbxxkop.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gcqdrxqtw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/geadzmefm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gcakwkcpc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gdwgmeceq.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gxlatfnpp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfglwqfli.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gyfqixmoc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/giazfflgl.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gpyctelnk.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gnxotexsn.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gzhdhuvgs.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gktrcbbvq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gnsifpjvd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gzvramixw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gapalorlt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/grwngipif.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gldeuiwkg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/ggbzrevcm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvyxvhfwg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gzuilprfn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gylabclyc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghdiwschd.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gbjqkvewe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gkhnseamd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/giypjfxan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmvwgnary.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkxbdwdub.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtvxyiwis.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gmwodktax.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjeejmqvs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grewleqev.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gutxnqbyv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/glexwpigy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gauziudoo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/geehpzrfd.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gpgwgsxfb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gtshazdcx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcekhuclx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/ghaydnidx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gtxhcwbsx.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gsnoyzoew.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gtxfdhvpq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/ghuftmsor.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gezslknph.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/ghjbufkyx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/guwgtaeaz.sHtML


<!-- 参考信息 -->