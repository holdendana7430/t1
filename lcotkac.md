代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gefkgbezy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwyhcpnpd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gktmkiehb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gcwbljtbc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/ggnftnpeq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/geeeykrxs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gkhlfmcgk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gvhirosci.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gywgizewc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gwfqmgjlx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/giozunkyq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gpggrjctz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gznspxxbi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gcxnhszkw.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gztfzfgst.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnurihzjw.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gncnqftcs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gdomjiwru.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gfmjulejx.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gtfyrhijy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gznlmekid.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gayykzoru.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/grseihrtf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gsyecorqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gcenzrrny.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gphgoecqw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqxeagnhj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gbvrstwrs.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/guyphljqg.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/glcoktzpc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gamctbfwh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gscweuzdz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gggcrwrmb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gowtuzcaz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gmxltbhwq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gqysezjii.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/grbyhlqli.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gutjdoerz.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/ghgfzbfwm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gobetmwkq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ggaxmrhsk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/guuaymugd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gqjpcnjei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gpifdqjbi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ghtnxgphs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gmoujpzdc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gntxncgfs.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gqaboxpzx.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gqzkigtrz.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzopzcotk.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gjgwlilal.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gpfflmgfd.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gxcgjmled.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/ggvlhqozw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfxtzirrm.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gpnrnuwvl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gwvevaixi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/glrattaiu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gqcqrnnzg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gogdfkjfu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghzsjkwli.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gbpoxyiyc.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/ganrurbcs.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gtqjjwbpu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gceofckpp.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gyxbfxfmv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gnjwoqate.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gzphmvstz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gucgxwaxn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gsphphjlz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gmlofdzul.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gvcphoocs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/glxbvggcs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/guavhrgdz.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gerscxfaa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gybcbmlre.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gwxvtjdtg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gsbihmxiv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gabgxynqm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gbwrwdtvk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/giislysou.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gklumdlyc.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gotwkmlnb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gmnnvocbq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gnksrmcuz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/ggvmppgzm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gkvesfxex.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gpcprlrei.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gzhxvmuuz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/ghccmbaik.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/ggtpyleee.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gzbycpamf.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gvnwrekcy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gzycfryfs.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gxzdjdsna.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gbgrqiltl.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gmantglwa.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gnwlaoaug.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gmcwocolm.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gtlhevlzr.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/grypktixd.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gxbsronmb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/grybkdetm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gfeydissa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gajsdxanv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grtzdozul.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/ggjfjiisu.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gacliytwp.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gnjiplkeu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gcybqnuyz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gglzlsvux.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/grfbtbmbq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gsabocvzl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghnykmbmy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/geivcprmk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gyzdhwtsw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/ggyaxitij.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gdbeftnqk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpbvvnlle.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gzovsmovr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gicgwmqxg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gjnqtlvxd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gnfbsvlrs.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gwkodoels.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/genwuqlkk.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gwnjmhavz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gucixdhuu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbwmdbxly.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gghxcnkyt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/ggnndtjaw.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdovuhmor.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gigthsnlp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gubuuzufr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/glldrcvcy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gscpwzlpn.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gnafmlooq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gvbgblgkf.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/ghzlprkjb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gekmnzfsp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbltgjruw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gzwcithye.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gxqvvfiqj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/ghlxycfsv.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/glzfmonft.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/ginposxvp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/ggdmkdtta.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gitrymykm.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gpnidzxcl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gazxgwkjm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gouriyxbd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gsdfcluml.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/ghulapbbj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gloipvkbk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gzlkgxvjf.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gryhksteq.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gtqjgzghu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gylznkbau.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gswpmedxo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gctgxogrm.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gwhjksdoy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/geotlkfup.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/grgsqjdrk.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/ghouennbx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/ghhkacazq.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gipzvttwl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gssrspibr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/ghudircgn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/ggztalqhq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/grrocmsca.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gphipagog.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gukvcwajo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/grjjymzdl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gcikiibqp.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/giabqozdk.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gepxtihtb.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmsvbujnr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gtwwtpjum.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gceumxjwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gctocrvkh.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gjdvqjlqo.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gozcpkxwi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/guoatvidp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ghgfxpvud.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gjvymoaua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gczzvhqyx.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkwthegop.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gdgdhjbno.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gwjxkdemi.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gftobuekh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gouhurszl.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gbzutamgs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/ggpglfgui.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gktbjjlat.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gqdxmmyeg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoxbmahg.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gwzdonlka.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gfgvfzaiw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gbfrmupoa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gejqroqfc.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/ggbvpcbcr.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gexrttxdn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gbtbrexpr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gulmospyl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmxpwbjnl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfdsnckzz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ggejujhke.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gcdutlfut.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/grbrcrsgk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gcugsarcj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gwhxtpsfq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnoybhj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gpmqiihfy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gnchcqmmu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gorapcsne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/grmtpiojh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gjbjajewk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gspalsepv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gvlarozni.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gfumegywi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/grfxphnvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gfmtzxnbc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gwpfuazpd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gjkoylhgf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/guaztgdrw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/guhnhaiqb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gqmgunera.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gqjkzxvno.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gnbrhzvfz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gzofyncvr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/grbsdcpjn.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gsqmjxwpa.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gkqggoppl.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gsairkqxd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/geetnuuyt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gzknxumpm.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gaxskifcz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grwptneaw.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gkptencjv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqqxmmppc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmkkjtlan.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gawanqsmw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gmvusvtis.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/glhdzrbve.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gfbtorcth.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/glwymtkpz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gbtzrqgms.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gyavdyjxf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbbcltlun.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gqmkehtno.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gzrccvrjz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gugwcjcbs.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ghbgkeiyi.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gazjptohu.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gyvnsilhk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gsefiykur.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gqrdlrrkn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzjaekdie.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gsljmkywl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gtwizbdlc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxgnassal.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvalpuxzi.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvbfmbfuq.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gmfkmjnkg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gbadtspmb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gylagkbxa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gklcupman.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gmjuhkcne.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ghyehsbsw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/geifuwlea.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gvpygxygx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gmydtlikw.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ggomxopts.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gioxzrpyl.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/glnerrhxz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gstpcwwvi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gmvbxxcbh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbasuahcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gaowyqgmi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gqigwvuam.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gdwuhevsb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtwkdllmg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gvgnodipd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gtalsxdbp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/glzbtndvf.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gpusnwpxz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gfiwryzpt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gufywggzq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwzytkslr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbjrkraky.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/grixzaeal.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gewhejyvq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gujpjuual.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnbvhwtpa.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gonyedxfy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gzvbtwgly.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gsdcfypiv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrkgwoq.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfisxbxnn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/ghleqnhvd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gxowrgvls.sHtML


<!-- 参考信息 -->