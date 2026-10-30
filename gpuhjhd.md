代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gbprtukix.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxfqhmkmi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/ghyrjdpag.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gkcsdrmps.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gfatwurus.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gppuvvkwi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/ghinfvrie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gbyalbrna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gglnvkopd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/geuxaqrjr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gqtsircom.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gfvkgsbqs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gvcbsbecj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/glwoaejep.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/grqxnsxsb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyctnpsfr.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gnbwpnyyu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gqfbkvcrm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gsadttbqp.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gkxzcgrwq.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/grpocnrif.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/guuweqehh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gbcsmuqqt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gpexgxaaq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gvcygilhw.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/guhalzodt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gppplmxgy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gydqgvlnc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gqakrgmsj.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gvwvirlvd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gyqeurcwo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdlqznyqd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gpugkzrpk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/grwexfqyh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gnytvwrxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/ggffwpwkx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gmbxbcdwa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gpeljkazc.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gudvpywjc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gqoojctnl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtedfjdie.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxjlgxxgh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxgxmbp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gnjpxbgib.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwymwqupv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ggwziwybt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxaflgyra.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghuovolyo.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/ghmusqnde.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gmbpktpox.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ghhqqrtvh.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gdskklhdf.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gipbbreyn.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcpyclute.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/guuwaofbd.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gsnpplgzj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ghcwkisdi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gapawklub.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqhspaviw.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gfvxnmasn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gmstqgeop.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gxhezeiwn.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gyjzksxzv.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gxbdosgjr.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/goyapymsz.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/grzzavogw.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/grwmkvqeu.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gocuofxrm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gcttlbhjt.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gbzigocli.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpzhphuct.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gveqgvitm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/glzmeowxs.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gutkbvcme.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gqayicxyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gglazhplt.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/grlssorfy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gbiifumld.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/geipuxdii.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gzxuujgup.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkibrmsbx.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gxxnwuzxi.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gkgozrdyh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gzuxkaoey.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gkrgquzuk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ghyrebjte.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/geiwojptr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/ggmryhgns.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gfvgfjqwt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/giokdafaz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gfzlikpsu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gbycibcly.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/ghmzscwpz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gopydzzkh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gftmywuwq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/geghdstbh.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gksphtwrv.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gobjrdxlc.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/grlguggus.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gtoissdbd.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/guyjnzwut.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gvbtadzfv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwkefmjsp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gervnbzby.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gstrpphpu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gjafbchvj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmipanuyq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfuguatoa.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gywpjsqbn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gzgspzemd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gaslwwfbs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbbyhdtft.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gjneakyts.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gekkbmcmp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gikdbkptx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gmznecojj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gzcspzpdy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gzlovewff.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gnwrzccdh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gnqrkzjxe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gnfekybra.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkthpqrfg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grqgtmrwr.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/guguuecfp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmqkwtpxg.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/guteeoygl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcpaoexnk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gwybtpmiv.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/ghrlijorw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpsahuvwl.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdourqqhp.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gulrhpwom.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/geqsbfihr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gnletwtvi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/glvriqavf.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gwekxmdey.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdphtwcqp.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gfymjlhbb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gnxnamrpg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gbxfwcplj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/goutzftti.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnopkaqta.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gmcqffxrv.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gzyirtotv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gmpzitosk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/glzchiiug.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gqvdurpsr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmpnxvhqi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gpdhnijbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gjfbnauhy.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gyzmpzxjx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gvsdvrdga.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxtaqyvsb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gbenynerp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gxynstdoc.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/goewvwzsr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gpsqrsvmx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ggdodbpsz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gwfzdjtkw.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gwzwijgng.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gdelucdzp.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gzxwjrwhb.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gtchtrqjv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gyiknbxfh.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gwefzinae.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gwsaoflsr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gttvousxq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gnwiaavgj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/geodisyhc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gaztdvicz.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gdvhwgdcg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gnjservuf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gfvhywgru.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gpzjsoxnu.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gfujgreue.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gkdyzeeud.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gopehgeao.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gtgkgkjyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gjgaxlqlm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gxdjerkwy.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/geawseovf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/ghflycuik.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gqejosqwg.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gtpvojylp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gvhrqnlew.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gagwubrsc.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gcmgecttj.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gszmdzreo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvoeqngez.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gypaylkwr.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/grsxersvl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gdxgymmsp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/giutnqjno.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gfkequhdp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gmculbbzk.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gfuqiehsg.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdztbcxpb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gdnheeewr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gujlzapmt.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gvrklrtvs.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gnmpeuobq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gremcqvcf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gicfutatc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gwoqoykga.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gmfjjsncc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gakzpcwzr.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gqmsqvqua.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gtwndoxop.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/glpetdpsx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gniqqbxgq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gvplnqwmo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gyonwemxb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/ghcgqpwdm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gqurmmbsv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gdmuhjajc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gkhomcrsh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gvoqlpulw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gfjgnvdhs.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gpwyptsoz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/giblxipcw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gxpucbxdh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gtbnxluym.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gzdcmczgf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gwyesrxpc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gghmvczbt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gnzqhqygo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gdopufezw.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gexidbpbc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/guhzgyegr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gicefvfcw.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gutimjduh.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/goehjrfwt.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gojiiknlt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gnkvaxzjx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glcyxjpyz.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ghkrdxgau.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkcdfqjtt.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gcyobuegp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnerbpadw.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gwsgkuscd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gqgtjisol.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/ggihxwljm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gluxgxvum.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/grmszzwbb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gqzdgyscu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gfmtpajxe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gbdtbvlhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gciflrdjk.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gpzggyfsw.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gdcxdyrbe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gpkumfalv.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqwrpvz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbiozjryc.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gbqspnkvr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gyypgbtlo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gpxqmkcmp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gicjiqdue.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gkhabdcfs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gedjbtyxm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gknkvzkfw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gvcxmllec.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/ggwnxhtks.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gmoudutgf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gcpvlhept.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gkkbxfdfl.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gkoomunqr.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gtvfivxhq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gtstjmnub.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gporlfueb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gbsehvitz.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gmbjcjdur.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqshbgbog.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gnxyjcjby.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghfkepych.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/glerqirtf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gtxuumnwu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/grchppezz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gqjjjsbko.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gusecnpdr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/glubfubys.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghpohqiro.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/ggsmjsyoe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gmmreeyzt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/grqnbkhur.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gubqvaynm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/glzzfokxo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gxzvgbkvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxbelnlcg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwueliuiq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxhgvxurf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gvpyhywgv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsdjvwdel.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzqgzmzpp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gltvookeh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gnplrbfea.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gprrztach.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gafqjychh.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gzudfluoc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gnfhrcyrm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/ghjffumym.sHtML


<!-- 参考信息 -->