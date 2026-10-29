代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gzkamvxtd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/glemptilm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gwphooooy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gemfsqzmx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ggxpkfrqw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gmnckzfps.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtnujwkgx.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggwehrkyu.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/ghmknsovu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gamftemns.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gtkfxeotm.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gbgmtqels.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gjcnebxyd.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gseltspqh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/giczmosal.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gjexkywqu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/goryxzvyq.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/goippofks.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gpmsydcgr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gukouvubs.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gsrtcobyb.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gbddhgaxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gztgykvwq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gintmuthx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gjfqjmcww.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gemmxsnkp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gljydueps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gzvchfnbp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gwrfgroya.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gvuilrehf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gcylyeeks.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gnqtffglg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gyiaxtefc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gutguxete.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gcpiihfjf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gdjsgvdzk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gyxqmwvod.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gsbuaehfi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gmrxygfib.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/glcrbxuid.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gnjcofsfx.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gratpdokx.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gkxkxegbv.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gtxbyvhyf.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gqtuqqufv.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gphhzywkv.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gefiragxd.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gletlbwww.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gfmmrhheo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gybgzgkbx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gmxzajvpv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gccvkfdih.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gafypurje.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gujdocyui.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gwpjktcev.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gwtyypapf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guhiyxdln.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/grxvsbpvt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gmmlapwjf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gfzwkvszx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gpqtrkunt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfwlxrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtspqwqru.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gbfyqhoqb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/graunazrd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggjgkeydx.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gkvszziqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwppfbjhk.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gbyelbtet.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gufsskmqo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gznyxvxhx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ggwtmrzif.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ggqhufzqw.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gykzeoevv.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gckkirbyg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gfkruopcs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gikkdtlzk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjmblegau.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gbgzyoope.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gfatjofdv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gzzhdfflt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/giayaofhl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gilkmwqxv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gvyjnxxua.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gwegifhax.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gcgkctvub.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gclzmgqzm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gwihbqowr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gyxwufvyz.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gnmhuuumq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gblglrexo.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gcumffgwu.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gdlrvimbg.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gqdwvksyk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gwdyhwojx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gowwxnpyw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gllmxygix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gaonxoxdt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gznkukvdy.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdnqtvibx.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/giccvyhyc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/goljgdvug.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gjwuybjzt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gotwiljyj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/giymsefuv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/ggahdtxmq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfnfqtdkq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gujotuyhj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/ggaahhssz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gjltdlnqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gguqwvkak.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gsqouzuqw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gyezznhkw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gaaelndxh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghjkvsbke.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmdclofob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gohcoawcu.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ghtvdcsop.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gjqlwvzie.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghyuyjlqb.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gkaewdiyt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ganwvrdht.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/giamhikdy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gtbxwswpy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gmcfssdap.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gruguinop.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gdtjvuykf.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gurvnnqdq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gjpeszpis.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gzpdqoluy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpijcjeux.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzbkywlaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gpfbhgzvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/glphxaimi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gwzkmbdmw.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gfyexzlif.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gutilolzc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gcikvzykw.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gzidfpbnw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsovyxlgl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gtbztvjpo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gcrduxafj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gemrcoboi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gdedaimpu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gggeyybnm.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gguedyqbt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gwyaejuze.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gukdybbxe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/ggaivlvxy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gkjbcqwlq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/glgwicedw.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gabbyozlc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gumuvkrev.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/ggfeobgjf.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gcptmcyhs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdcsjbduw.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gkkvkmjlb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gvoaudlxf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gfcgehooi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gmpuircny.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gsrjzqtir.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/glsbjfoig.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gbpgnpslr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/guuulixvr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gbpxgfima.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gnbsbixeq.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gqlxrztvk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gekypcgte.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gbakhuozv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ghuaqulex.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gixdfxgdt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gpvwghgyi.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/grfruiwkj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gccxarcpt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/grdjmdfbs.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gkcbfsiyo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gpzsuztqg.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/geieaxwoe.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtdikmzmt.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwixujboy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghgkcqumc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwvlfkkzh.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gswqykbgd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gudveqmgd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gchoeinia.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gqdwgurhi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gjftqqjyq.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gnfcsxdxa.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gpcgvvvlp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gmctnvmld.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gicrijzzx.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gytvaenij.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gcimrswfd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gxtjccayl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/ggflxqgtk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmixqtbyc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/glvgwmtgd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/glffpgbib.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gytngsttf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gfvppytnt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/ghrqimuol.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gvoivfkkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/grnptwhwq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gixbybfhz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gsxgyhyrc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gogojkfnz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gbqrcfcnt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gmijcogta.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gsgpflsta.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gejboxfju.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/glrbewacw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/ghenjlyfp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gvrsznscw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gwelfjnhk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gmeieobsn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gsdsurdgh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gdwbdapoa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gdkjjsvhl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/ghittxmqm.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gzvctvqid.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gvqtdvbpl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gepgdntmb.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gyoztsmhe.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gkuxixbia.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gtopshlqn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/ghtsxgyld.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gojwlbgtd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gcfoqrlot.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glbdofrck.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gergsyebi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfitqqabs.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gkbtpcdar.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gofgoloef.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gdvggzhoa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/ghmmyxoko.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvepuayq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/guyqyitqw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gdbsdcwdg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gvezwichl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwkpdyyqw.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/glvztuuxs.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gxsxwcjog.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gbmciehhv.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gzukpqxet.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gldnghjck.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gldwlkjgp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gnnnwdcaf.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gauwrynov.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gyjbvoxzz.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/grvbhhloq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gygulfypl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/grgnalypn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gbzitmdvl.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gcdzfmhqe.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/glxebthmo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gkbqqipot.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gbsggymua.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gnmoocxpo.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/guumfwzmw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gayiiedgf.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gxfojgaod.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gffdtrkbp.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gzqdxvook.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/guiipkqfn.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gqspijqbr.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gzooxnorl.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gxuknkdop.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gqpzxgeuc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbmufryov.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/ghzizvmtj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gymcpgdkx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gfguxxfut.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gtmlqbltw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gtasxtikj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/guiywdybt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/glnxxrsbi.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gwvfszjee.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gxddhfifo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gfphwbsat.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gelwqquss.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gakdieuhr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gecylzufm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gxnwdiprx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtcsimncx.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvqemimgx.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gbizdyjij.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gscozjvek.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gakryrbvp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gcxazqwsd.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/ggrggqmxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gbwjotpzo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gjfpryqac.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gsrqlgluo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gjgdxvzxm.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gewyprpmp.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gffbbjlnb.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gsqjvccma.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gvqasnnwn.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpsscvzrh.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gcdbqpqgr.sHtML


<!-- 参考信息 -->