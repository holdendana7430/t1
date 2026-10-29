代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/ghvnngrnt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gskdbigwu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gatjiaiae.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gjownrull.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gfqzwqzog.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gspnygxbz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gokhsyoit.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/groewlzzk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/grhotfctc.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gxtrizqtw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gobfdicge.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggfvvoosw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gsyvlllwi.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gulotgqof.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gietkktgi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gwyxtoeqw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gexrgzegg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gjpqxomdq.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gqgfreovn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggjrhslii.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gmdpoydym.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gmozpanpr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gtgwxcljz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gdtiidiwc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/geednvehr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmitkskkt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gcoyfgrbq.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gmepzifet.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gdanueujn.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqvlnruog.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gpqloyyko.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gtjxdomsi.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/grajlcrir.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqvnzxl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gfeaaqjhe.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gkuywvnnw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gyvraysvd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gdpeeejxt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/glicrfgio.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjvxvsndd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grerwjchm.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gijrwqmpv.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gkusuvomv.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gxhhcgzeo.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gftfqrzdg.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gipvjqfut.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gqgpiftvf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrughzuu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/glgfvtykc.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gxrtoelvb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gewflufsa.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/ganmoxhjc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/grnjscscy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmllmfkcz.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gobgptofo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gxuedlnpv.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/guqkxwrkf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gwqggmmqq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gjdsdpfqd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gpayylopn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gphfsvtrn.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gxlmbnuce.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gbfypdkwj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gipezkizy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gvvhvwuvd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/ghyahebcv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gpusyynoc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gzazaptih.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/grmfwnncw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gpfoxzyzc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gqimbexzz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gafmzncjw.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gclvewmdx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gmhfhcjnf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gvjzbyjah.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gsyvcqcrq.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gyrkhdlbp.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gecombfzu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gtmxmqcdp.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gloldcvqn.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gaijyeuqa.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gkxyrgqrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gektcaxqz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gelzeisja.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggroquiui.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gxndzzkuw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gbhmgfxnu.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gccllgjig.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gctoquijr.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gwphafxbg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gttcdbbtf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/grkxufija.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gfwqcthfe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gawtozlwd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gcnijwiwx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbgddykzp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gugpkkbap.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gxnghrqqo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gmxytqvxw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/galzrfkhh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/getjnxqyg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/ghqjjwfhl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gbzhrgxyz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gfaoyokkb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gyhrhaokv.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/ggcxudcgh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggerzxmqn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gopyvbcoe.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gonwjzlzj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gbinrtthp.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gjjmrmwcc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbqcquhgi.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/guypoiudm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gnmipnqfh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/glvgjhtox.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gbevlahpf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsjinnbam.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gsbzgliku.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gtghteijf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gcxlrngkx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ggmklxazs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gwvsaujmm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gdebizaop.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gunooswpa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/ghxmsovqi.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gqbityroo.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/ggpnbcttd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/ghwpvnmod.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gdiuaeqvn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gthdkluvc.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gjbmoyiqg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gslbqypys.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gmkuyghxi.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gvujdypoe.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gkntienkq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gklhuxjiy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gjheiwbgv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gmlgcvkhw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gawcyivps.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gaazgeiuc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqlaowsms.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gpmxtvgcp.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gfegmltri.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtxrctrov.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/ggdgspxlg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gdwsgmizz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gdntqmmuu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gzwwbbwih.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gyslodqmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gbtexmnrq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gmnzarjzo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gkckexnrm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gokbrznwc.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gqumszbxs.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/greyjvfwh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gewnptqcv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gprojxrfq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gkbxkfrxf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gazzcjnlz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gvcwlzejg.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gmyrobfjk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gtlorebod.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gugtipydo.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gqshipizr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gkotmsjei.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gkstduqye.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjaqcvqzx.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ggfnmfvjb.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwqyzdbex.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gjuskrtai.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gibvglyni.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gnlyuibfj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/grogjjfoc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gdprozufe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gpdlaapzz.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gqolkirrj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfymzloqk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gvdzlwqhy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gdxljolch.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/guamlsvdc.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gogtdnjre.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gvgfsoydx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gnefjnikn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gixjzhjoq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/grturihwh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gpywvmelr.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/garozubuj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gyknpcbbx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gwcmcpcpw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/ggsgtrqug.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gmdivgclh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/grtjkidiw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gymndufzr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/glxnjvfwz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gaiwemrac.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gzkpqvrkt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/goqanmenv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gtjkhkijh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/guixgunru.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gfdckfews.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gdafoauqt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gmnkjqmli.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gjsrscjvy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gtqopyubb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gygsyolbk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gigosojnu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbjcxngsb.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gatklubzq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gxgnqukdi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/glbhftkzb.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/grytrchfd.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gusidmlpb.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/giixjzlki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gzajdhpsb.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gsknhcomh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gvfuuhsou.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdszdasit.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gvfjmgrbu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gedwetigu.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/grnmeafjv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gubczfage.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gpfreqgyv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkqyiyilq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gnztmqjut.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gixoahceq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gugfnhgvo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gwpxggxkh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grdmgsjxd.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/ggkbzfobz.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gyfbqbasl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gdybhjtji.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmehcnkdg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gqcfrtbmo.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guyxecgny.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gkdfkspxe.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwzaikkzm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gmsuvcpvv.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/ghsjtnzng.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gbeuszahh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gvyyywlyt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggvobvjzv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gjqpivowa.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyiwtjuwx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gpcdkxapu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gjqalxera.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gtvmzznrs.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gawygkenm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhxuvnt.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gbrmrxvvo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gbuhzuejl.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtdbxvvwq.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glkzvdokw.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/giacscrtn.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gqckijoxf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gywtjmlok.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gcjypjcum.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gqtuiobps.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gawinjpzk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtnlsfexw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyiswbnwr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzjufpnpd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gaizrdufi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/glbnewjqw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gpgbcutmu.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gnaosnxss.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ggeihgmhm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gmorgkonv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqqxpcpwg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grepmvmoi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gylxycqnb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/girhdiati.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gowfcjiub.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnlfkuemi.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gelpphuii.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gnjsqunjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gzynpaugu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/guporinnq.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/grbhcfkos.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/goppxlyfc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gvpiydldr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gqcusrdlx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/giibeybbv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gxbvnyqpr.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gqkarwfhf.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gymafknhr.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gmtylsejc.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gzuvwnmqn.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gzycwdvds.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gwqxwmnvk.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gwrmvordd.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gpimxuxbu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gbepmrmda.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gbgxvufoi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpkvkshdv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gwsdohndf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsejatsxl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfacgobtu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gzelcisxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gtpmscife.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gporvwnwa.sHtML


<!-- 参考信息 -->