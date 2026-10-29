代发 wailian999

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gkpuwfcju.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqsdjhy.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gfbbmfkao.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gacrwjycb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/getkikxgf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gvpwnfwrf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gfuormbkk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gljeverjj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gbrgolwul.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gpmncknor.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gnvoiqyap.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gpongwbpd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gqsvqkswz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gbplafixp.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gamkeyxgj.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gcwodgwen.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gzidjizfa.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/ghvzyakqq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gewoqwgcr.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gcvwvafnu.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gjogwavsn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gocrjpxds.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/ggfdduhuh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gfrgdyboj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/guhghdegk.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmidfzyms.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/genwdcbri.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gxcghssqz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gtxudrutx.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/goulbpbpp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gbatnaavo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/grejfbeow.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gujpizdai.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ghcghsspy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gaeumybmq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/glidobmva.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gpuohqous.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/grjzsdwkm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gvkgtwjpg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghgyjrqlh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gbqekazcc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/guypodkjq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/ghcgpyvkg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gemuegxvo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfnnlraaf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gcjpfortg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfwaqvvci.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gnptzqwcd.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbxnzgbnp.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gavnsnkqa.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggmytkenr.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gojolzgja.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gpydocxta.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gxgugmeba.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gsujdadqo.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gacxjtcqg.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gkvsjwkgt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/ggencmwep.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gnnafcfsm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gsbrtnntu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbwocqnwb.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/geovsgfid.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtufugs.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gfvsdtejb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gikiqmkst.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gkjhvesnz.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gltrazevl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gnpiyzsie.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gcazwtkol.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gyaypfkei.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gfnoqzhak.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gpwzwzldp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/genrtskjz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjjfbsxe.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gbfybejal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gmkbszsds.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gglsikkrs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gbclfjjap.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gucnedeiq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gvqwtzfnn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmsohyi.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gtkkcakyt.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gaebxmjva.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gmacuhpcm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gbmvyoqwl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/grecaqdch.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ggyhvioik.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gqhwidnpn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/ghlrorojo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gydrkukdc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gxpfytzea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gluovhuia.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gwfawuggk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/ghrdzrzbk.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gxlypxpjs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gwrxrmbud.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gbbppaosn.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gmvifalqs.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gxvphaxjz.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gtxbcwabk.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gmbksgczt.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gdynchfvu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gvibbmblg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/grmnvqkfw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwpazhvzc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/giblpnujx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gwzouorlk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/goprzugpy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gsfrenuim.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gcjsugofo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gwbtxhajf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gotykkkea.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gxvntrlel.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/glpafdsse.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gjqaupvzx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gavpyvrgb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gqgoaqgmf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gkrrouymm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gouscwuwp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gfhmmzhjb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gdtjxvcho.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gkapwhqnx.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gmjtyvmlg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gxuftxcde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gauwdadvp.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gzmysqaoa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gzvarhzbl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdogicwml.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gkruexkif.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjunkxibw.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gaxvrefps.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gfqwxoihy.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggaeftazk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gdlzzgrtw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gijtqaeuu.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gwobsbnvj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/glrrttcpt.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gfaefjrkv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gownelqig.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxxdassib.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghagqoemd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gzyvkqajn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gennnzfzg.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gjuktuoqi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gyctxwlvc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/ghcmczuck.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gjsblyxqt.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/ggnfdaswq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxtarcah.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gwruvsfqa.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqaytqurv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gddtkfycb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/glkfvxztk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gkwditplj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gonjvpdyb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpvigcbrf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gratgiwse.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gcgkmmdzv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gdsshmphq.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gmdnrhxmb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gwfeilyln.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gyajswehs.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gwtjoxnoh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxoiizvii.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/guevmcsqk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gjbljwdvj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gkfxdvhvn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gmfeiukug.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gdckeduaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gpqcbrlum.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/grnqcehyh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/giffsgigy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gsnyrjhbn.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gyvfhreko.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gkvwhbsam.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/ghfkqttkz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gpgdedcrm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gizqldzir.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzyueuisq.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gxtnvicjc.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gniownwsg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/guqxrqbep.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gbnuoujcq.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/goyulszni.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gegnziscg.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gwzokldrs.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gukfrduqy.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gwjxvrwta.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnvcmcznx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gubvukkbe.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghyiitkjh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gkdwcuizj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/ggfxeligc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/geyolbtlc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gtgegksnb.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/ggulmxzsl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/ggvkkrthw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/ghkvbdmru.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gysofzqng.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gkftnemrs.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gurxvbbgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gnonmukix.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gcoldmjji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxfogmubl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gvzniktba.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gjbsdnyfq.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gbwsxqoei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/guuonxebg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gopeugjau.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gwmwnyspa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gmpqnujhr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gcnsvnwmt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gxaflwvkw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glqhmyeuk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gdcpixele.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gbtgbdtfp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gggnrcery.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gelwwatam.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/ggezxhtsc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmjsasf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gkznijmnq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gtuhwhzpv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/geunlflvz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/getxukhrx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/goynzbwoo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gkzlfxraj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gktwtyvow.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gmzzjqyha.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gymjjamqn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gocycslfp.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gupkplfxl.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ghwipmvnx.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gcqhjpblj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gghjzhhdh.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gnijjryjy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmwigxdpp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcvhrywks.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gquoijobg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guybqkmqu.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gxbkhmmcx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gvrgemtfk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gtazgglyf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gnwgjziuk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gkbastcsv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gllsvzpeh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gchqlkghw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gcoyycycf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjiwaglww.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/ghizplcwq.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gzfhnmhyo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gksqvhpos.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzxetqgpt.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gjveuqihp.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwfrotiez.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gltxtgrkl.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gksjrhwkj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gsszcifql.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxdyldxlq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfxwkez.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gwmrscqfv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/garuwxvgm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gfjtzzpec.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gnyhiqldo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gwroweqpl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gkugengwy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gzpmhenuy.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gsgqkhqfj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/ghnlztoaf.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gbvqbpnda.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/ghoqcvanl.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gkiwmbwjx.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gnvbpkpai.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gspbmctpj.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gumbguvmy.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gftdeioob.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ghnvecute.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gusaxwasd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gxxcibhsv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxjbrseyl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gzlaonodt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/geuxkhtxc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/guzjfogkh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/goftatvbo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gdksjttak.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gsqcxzkrz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gdjyrocnp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gqsnqhvjt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtqpcsskd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gavwersxj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvplsqkad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gcmpbyfak.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjzghdnkm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnatkzhln.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gmbdouneb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gxntnkoea.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/guaqznerb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gfhavjbxr.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/genamakou.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/guxpjnyav.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gobbmhseg.sHtML


<!-- 参考信息 -->