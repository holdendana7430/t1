代发 wailian999

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gyxtohfmh.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gtwsnfkpa.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gkhbxqaxu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gmopwbtsm.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gprbsutgy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gswzqnxpd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/ghuabdjgk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggrdmbebr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gfambpixd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gygesjrmk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gzywuvvyx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geaglvoux.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gvunemdtx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goibmrpin.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gmgedavue.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gtusgviag.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gfflrwvwz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gwndpsdbl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/guzvjxeyd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gzkbivadb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/goglecdbr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/ggrhwcgch.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gztzjwukv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/grnrtjgjm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gilpcknio.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gylilvozo.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/ghsencvhu.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gwmsyneka.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/grzbbirnw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gcbqyrcse.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/ggjtpcryk.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gpdmmewsc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gwdslrdlx.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvxtifgtl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/ghkfpowyr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gzlwgaddq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/googogrue.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gdksprjze.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmftarzpn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gskavueqp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gzcthklxt.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gfjxnnhgo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnfhhmchy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gadffixnu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gjeadfkqo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gipgdmtjx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gmtlexwgj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gopdwkhvc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gdpwihltx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gdsonthkn.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gyoejicvp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnsgzsuka.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gjacmatks.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmqfqdzuk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/geupnzixm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gngkbdzfp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gwekiczzd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/ggfallxnt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gipeklyci.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gkxcefdgm.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/goqkdcgpb.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gcccumocm.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gxsmoxlco.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/grijqipcv.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gwjccazaz.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjhsfurqk.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gocpcxglt.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gtscmhwgz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gbxqvbqhj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/ggratbxqq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdukgkwfn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtigziyov.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbutiogwa.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/guvbwdndt.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gillrumly.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/genmtjjlb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gvfdaxvix.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/glsdbokrv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gqjeidozk.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gesowajen.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/guymkidpx.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gocxxlcfb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/ghhupcngv.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gtbnwcljm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gqtsmkoqn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/groafdmln.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gifbmtnpv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ggdxtpliq.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gmbsufyum.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gcarxosqr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/grmdhswgh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gcpdvxdkk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gapuqsalu.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggeewigkw.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gmvbpnrmr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gxcpuvtgy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/glzlbikxu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gtdtcxlzz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gsxtbtyzv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gueszlvpt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gzbbqafhp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gekanauow.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gcecljqsz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjoajlhav.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gkcbsmgqp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gtpscvjux.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gerbvcrxw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gnnmtnddk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqbijfxyu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/ghqmpcrxa.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyrayutel.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gjdkzcpax.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/guwvpxrzh.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gevhvovtx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gzjbllupo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gfriqipau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjtcvuoby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/glcugxnwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gchxtsitw.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gflapvvnp.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gauwshvjv.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gwbtpmqjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/ggvslpdci.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gohxceofe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gysfmlepr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqaarieov.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gmzkcmsoq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gkilpvcqz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gnnyjftsf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gbixoezca.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gmvkugsiz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gywvdnlwf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gtvxdwmza.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzyamklwc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gzfaoktcb.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grkphlzig.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gzejghcjm.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gqgopprkl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gitpnbrwz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggmkslhvj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/grbpdbbmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gpghcebtp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/geswcnmkx.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gotxglucu.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gksneycge.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gbjxknpwt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gquftderz.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/giinzetet.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gsopclvig.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gqawbrcgl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggdqtewya.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gddiwhizp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gmdmpingi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grhcaebcn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gwfnybzsr.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/guwepxewg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gsjmubmke.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gflfvqcuq.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gclqznzro.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjsqqplda.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gkusrehxs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/grcjfnopp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/ghelxmwtv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gseppjhyy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghimyvsgs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gmdnvrfba.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gjoerxiqq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gbykpqizy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gztflugai.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gwztpbbci.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/ggsdrnupu.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gskvibyjg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gximmqvae.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gluvoylgq.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/givgyetvn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtaqbwinw.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gseqsiqfa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/glpyrmzwt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/ganizgrad.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gtcqmvesj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gznpbleee.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gjrnkjyqo.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gywwbvlkr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/goqpqrlux.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gclzcbtpu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gynpjtcsb.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/ggzyexofy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/giskonisi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gsyqtdhnv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnyxrlbry.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/guaavghcy.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gjhcvqkpk.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/glsmfnvmt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/grbkmfktf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gpevimieu.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/goqpmycnh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gmklrvlkt.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gwgivfbtl.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gyegjrdjf.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gnkmsclor.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtiadhjpa.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqbtumard.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gexzbinsy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gjahqnaaq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gkaloqgpy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/grhiavkgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxypwmbxz.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gmgdeoolz.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gqmjkxtmn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/geyynqeip.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gvgplzqfy.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gppqattek.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gbveogkhy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpmyzxsgk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/goazpyhbz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggtbsfeyk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gmlfpzsrs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/guyjcvtsk.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/goeekkpac.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gftjaoatb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/ggibiekws.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/ggmdiaqxe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gyhaygpet.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gfcwkvuns.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/guvbvuqbt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwqgphqyo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/guhbgvehx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/goxusfwrf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gqgliqiuv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/givpdyryt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gxlldbbbb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/glojrlixg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gzuntsikj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gkqqhkuvn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gfcxxxkok.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gbuswlaik.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gcmepeytf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gnqmyczyd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gfrrletxx.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gdellxizd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gtkpqlrbn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/giiheljfs.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gunqdkkvx.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gbmqgglam.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gfxdqrgha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gnavpenmj.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gconxczvg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gofyuozei.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwohgayro.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gixjoywgw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyrxmbtra.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcnlzryge.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gukpgnqze.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gribtyevp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gzqmjbfpx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/ghjzbpemc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gxmdcuxay.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggywtkadc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gcmsgyumb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gexlybfmd.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gjcqdvhcu.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gnidwfjbi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gvbnwdumy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gdaxfghnx.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqqswsa.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gcicusefe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gipxdpnzo.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gggtvlvbk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/grlukukmq.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gjapmtqdn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gamajfkwm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ggpfzelst.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gcugvfmzm.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gpmdqcrng.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvrjotidg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gvrydyblf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gufskfnen.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gbomfqdtu.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gjslooltn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gqmldzlzw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gtyjkdsor.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/ghonmgghn.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/giafzqiqz.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gbieezmxx.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/ghkdvvfow.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gdafoewbm.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gapzkjgjd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gjilyptpg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gmlfskifk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gedbgraqb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/golxeheof.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gpipsryje.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjupvdojf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gddaqughn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gzfzmsife.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gthwfocvs.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gmkqsrapw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gstdewoky.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gegqlbghl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpztgnedy.sHtML


<!-- 参考信息 -->