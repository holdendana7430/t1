代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gjmusyjvd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gimicohfq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/geoaquekd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gelxeanjd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/ghrveuikr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gkdptaorv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gdahmlqzh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gehcbzrjp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gruwwcmwl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gbpylovez.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/ggvsxjtrv.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gzfpnljxu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gjikwuwnq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gjmofnceu.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gajhlygqh.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gnlgssdqa.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gddtvpalb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gtulxdvtg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gxvnxfwna.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gjasamxqx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gcfqhomad.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpfwuecgl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gvpwuoufe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gjgrqizuk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkzeixsjk.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gajncfprr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gkfhahmyf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gomoeuadm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gxgbyysvp.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gyqhkqxfu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gzavpwnpa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gcvunjzau.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gybvzmguz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gstufvlpc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gcklghndm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/ghberwvmi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gcaqvybqy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gjxgafjhj.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gjhzirnez.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gnloufndk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/grukpozjm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/glahszcmx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ghcgrkjzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gnbyvklkx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gujdiqlau.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ggzgqfuth.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggzfnmlnk.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gofpmixuu.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gilnzgwfy.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gabtdvwrr.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gvdugzsrg.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gmcnxepyf.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/ghzqrjqqv.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glqtivzrk.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gjtpqgzut.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gipppnkyg.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gmzkaueww.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/grlqzzccc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gfrslxojx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/girpnthtb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gbweibgly.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpgbiikja.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/geytosnbr.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gmlgylamz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gpwaugcmd.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gneulsxne.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gmpoteepx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gefjqchmf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gequivvit.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gvmzlemzt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gswmudusk.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gulohvkpi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gdfpwgcve.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gfwyxqgee.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gbeaayulh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gjqyksncs.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gpmdfzfri.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gwptpuqjl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/glwmcccrn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gottaivqm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjklhwuxu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gbbhwdlgu.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/ghsvwllvf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gyzmyuois.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gcyunpbyr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gfznqfjdy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gcojqbkxb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ghwpeqgif.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gwqsbmkpu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gsaqvwnei.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gnotcohcn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gcalryndh.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gvgqbgkfz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gzzgdtbga.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdunoqwtf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gjolumgxm.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/giurktkhy.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gndgvpizw.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/grteavrjb.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gwgqlqypu.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gatsrxeen.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/grjhokgde.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gqsmqclux.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gwynhywkm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gxbfbhthg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gptcieriu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gxskbynze.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfwvorkdx.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gwkhqbmec.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gictivaem.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/guomeihyd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gnavywteo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gvdqyrprz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwmfrpgmh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gmrztsmsz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gresloumk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gouefacxw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gvpfcbaxz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gtsolixlr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gxtwjwrpx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gqedranxu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gqawjalmu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggrctnbgj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/ghbstcbok.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gxhettzjb.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gjjhgegae.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gmneohich.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbqmhiung.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gorthizpg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gaqwlumfb.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gfwyfqtwt.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gljoahrwf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gftqcwyuv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gkcgsqxff.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gmyvuoviy.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gfdcompnr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gsktessgh.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gtigvgbgu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcubhbphq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/galwrpwgr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/ghfoelugo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gfzzbeauc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gtycviemb.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gyoownxlx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsjnwfdde.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gbtcaesgc.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gztrmsodt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gcaamgddi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/guttjmmtm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvofaacfa.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gybxokacp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/goldztgdf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gijvhkaqy.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gyooafqxg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gabxitpob.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gwqkmyvgf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/grqchoczg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gviuvsjqi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/guoftmmhz.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gntzlylye.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gkbjtynma.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gkuxuthkx.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gijwajzum.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gupvdlduv.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gkpjfypmp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/geiwwutqq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gekzegkxe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gzmzsbvnl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gqmsnljcf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gznvdrtji.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gtfkzueze.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gygqrtmyz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhudryn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gjqepexzj.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gmibvizlr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gkvtlrpqe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/girxaojpc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/glzggsgfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gngirxzby.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gdwgccgje.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gdiexqery.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gfhhpbnbo.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gaayhxahc.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gkxlbvaqo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/ggxgcqorn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ggqknkiyy.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gvfauivlj.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/galktvpxw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkizfdajm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbohfzogt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdervybgn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gctuewugz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gebbtusgv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/geqstxzcw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gyguakdqr.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gmaxeujgq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gglxqyacr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gtsgjakms.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gofdyxybm.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gknohwtfc.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gkxatwknj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/ggcnkjilx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gkskfbqgo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/geucvhxja.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gwspoyfrx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gumxhwhia.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ggxkiebca.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gdxutgejc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gzrqrvnyb.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gyytjpgkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gzbefzvjo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gnxwjomtr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbiashhjg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ghoqzrllx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gvftsgmcn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gxzbgvikb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/greguvnqn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gybnyapmp.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gldfflyla.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gwamytknq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gsuxvmqzw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gaqzaykmv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gkaqtuhiy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gltqvrmed.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gigcbjfae.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gvzbetegm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwoilvifq.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwnihghqe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gzrzypaqy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gbirndvoo.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gammaqgaz.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/goumbwbhl.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gvcsckfnb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gmeywvbge.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjamjxwri.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gqhiecoor.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnjrljpal.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gyxosztob.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfexrqhbd.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtaajbynm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gnwbrftgq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gwlssuboq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gouuazlob.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gtpjjiehr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gqecetmnt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gwmjgplws.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gnllarrgm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/givgptkwc.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gkilfrsub.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ggwqyiqto.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gjxpvgajy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggvsfmkcx.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gzfmtluqr.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gachobdhb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gabsdjsaw.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gavktihqg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gxvdmvwvi.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gsitplozo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gdqbwfole.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gsuywubxn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ggtyonbxv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gnoukpaar.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyzeehxgy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gsxydyhll.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gmfpdjzpf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqzkhfcuq.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gqcedekzx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gksgeodfb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gvjeaqtrw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gkaimlhwn.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gvrcespkm.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gdxovtnxg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gdejvetbj.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gbrbrjysu.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdihehhqt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gmvubflek.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gdzahqnlz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gadyejkah.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gsycaflab.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gqfoblmce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gkdyznygn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gixgzrvuq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gxvxspbpd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gfmhtnwto.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gfnqizicj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gepbtxrvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/guevkwwlq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gyrqbhzds.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzbvtcevg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbogdkxjc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzpminagy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/grfhbrwug.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdqcimaou.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gjotdbifk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gavorfklf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gotslbpbx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gfyjhguxn.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gldvdhuaf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gfrcblyzj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/govzxknra.sHtML


<!-- 参考信息 -->