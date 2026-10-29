代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gxvbwrqgs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/girmtjwgi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gkbhytgie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gwwvmbzne.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gwmylxdya.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gckbweslb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gwopeaqly.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gllbvfbqg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gywucxhsn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gsmofqmsn.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gjdpstqyq.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gibfdonuo.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gtcjjvbiy.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gbxsmkxoa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gbnofcfyx.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gejjhunow.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gkrkbezls.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gsliiejiw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gepqgdrsw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/ggvojbgbc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/giwdzrgag.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gcefekxkk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gcugxdtxk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gcrecpsdj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ghmisimbu.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/goariqlyq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gkvcsbjbn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbresghez.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gtmkdhctw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gpnirlxco.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gnzvlajgw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gjvemwdwt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/giibdlbcc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gsrsdiwkc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gliyqpnrc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqhmclfay.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gysrweuch.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/grpldtyth.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gccrqjplx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gpgdguwvp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ggejcjexo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghciscbwc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gfcsktsbu.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtgbgsbls.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gnrzusqda.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guctiuwih.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ggbnlzpcc.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gmgwydnim.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gmhfktvgl.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gunctdlll.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gjvgenged.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gpdohhrrc.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gnivptcdg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gwrsknthy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gvbsbtzfu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gpmgicdql.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gfjwvscqq.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gcyrhdxaa.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gpuanwzis.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gtshzqlbd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtuqkcauj.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gaolnttke.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gucwqkngt.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gybunknts.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gsktmfodg.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gfzyyejly.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gaokbcwnr.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ghmjxitke.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gxrquyjkc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gdeijbrtv.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gfrtdlhfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gevosgtwg.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxjdxxqpa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gzwvpgrlq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gvgyfxhgv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gsbnkxzfw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvlkffirr.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gizfyiwis.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gomsaqtlv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/glebrimfj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gxmstqewx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gokprjljv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/grlsczjre.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ggdyqpjbz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gaqltzssd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gacayvspm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gqlyiumja.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gugymsmhp.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/grngfwtuk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gnlhqwrni.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnimaihmz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gllwfablf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/ghlnoppet.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gfdmectzf.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gdkomnolz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbfvfyhnu.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gbypaoyhu.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gqtxpghap.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/ggepmgggb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/galytrdab.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkyqzslvq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gtftksqqo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gmialuwqz.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwvttezqt.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gqazemiuj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/guriidsvt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gttxklyax.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/guiyzumft.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gqpoeangy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjlouhjnn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gomcmwymr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gvskpptdh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gapihhgin.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gggkxgorf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvxnnuewe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/guvuhclbu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gkasvkwfa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gvvpzmaux.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ghuoimsya.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gyersfxju.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/guanjjfzs.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ghkeukhql.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/glexkzxxm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/ggamjomoq.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gsukyyelj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/ggilfhfsr.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gveiqarsu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghlstihgb.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gaabiaawt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gcsnncrri.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/girbiytqr.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gukqqkcjq.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gbtiaozuk.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/ghcgcraoa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gieahttlb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gydgqqkib.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gcmgvydck.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/ghlicvfkk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gkiixfcap.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gnrfhosxb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ggpziqoow.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gmcdjlfsj.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/geptzppct.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gtlrghjjw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwragawgv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/ggraaimqr.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gjqnyxzyl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gmcpfbbva.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfxsbfkvv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ggqflovnk.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gdrkbsuem.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gjgmuvjpn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gdbdeogtf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gntnyiuhb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gldxhgzum.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/grupsrsyg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqaqqoztk.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gykgzssat.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gvmlhnaie.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gfhaiyexc.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gzxqizcby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghmrwzlhp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/geuqwgqbj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/ggetncpib.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ghcqqmikp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gjpdehhgb.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gupkamsjj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/glerbolfi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gmzablkpl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/grwvzagex.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/giucethup.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gujppuewv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/grliltole.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gjzitjpnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/guepogyec.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gccsjttsa.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gnawywnwr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gjazmwjzq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ggamcvebj.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gfkithtzw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gwnuycvat.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtuyrxvfr.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gwbnzodwn.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gxwqjemit.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gywzlzeyl.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/grphmrdmw.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gufzinezw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/giefuzuqn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gseaikdlc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gochgyjlg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gsypksaik.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gfxlcjjrv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gajuzzsam.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/guyhfrqiv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gosycbqcb.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gyrkjapdw.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gymjruccq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gljymccue.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ggesaenmi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gedyfruxy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbofnkque.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/glgfjzfyu.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gsemlomrj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gxzpgkgcg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gcoiruryk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gxlimwjwm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gteetukex.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gbsuelbew.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghaafpzqh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gymbppbhj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gsbkdxwqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gsiknvivx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gpmdswqct.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gjvchvghz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gqhlsrraw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gvetxrjfv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfjvmounn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjcvydayx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gxzvdfhka.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gzianzckr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gefavkssl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/giugonbtw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gmunjcntp.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gwgyyoxxj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/grzawhtvs.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gytgvpykv.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gscjcvtgo.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gojytzeoq.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gxpwzpicv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gtwzxdunq.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gemidzbqk.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfummppm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxwljjebh.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gezvsgyzq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ginqejkhp.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gryznhgcr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gptkvjohn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gbfigfakt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gdenzysgs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gbdtzlacz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/grgtgeolp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gelckkvxc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gcfnbqjlw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnhkwxiez.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gtmdsyqtx.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gdbborzpw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gjvtojtzq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gsavxzwyt.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gjztjaqas.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/govhkhvht.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gadgiunld.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gduzsqneo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gziuxhhia.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/guhftvzdx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gcqmospwp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwpapcrob.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ggzfpifni.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gyuodaooj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gububtkut.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gadkbhqhx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gdghwrtxl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzysjlrrj.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gctzrgpoj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gazzootjw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gbgjffvrf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gisdqpueo.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gzoopniru.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/grxuotjmm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gsnjpguek.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gjerkhfnv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzkkipzqw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gkhfbggwc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ghjyumivk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gbyhnyiwq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/grpvqfvpd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gozmcduud.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/giswkiwmt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gccfqsgoz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gqlcakjdv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gnhbuhdcy.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gzeoeheqn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gcowyzbre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gbsbhijze.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfvyaehmv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gozprmwki.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/ggsmujllf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gfgaaqacy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gyeuribpn.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkarwtexf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gblkkovqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gpjggqgrh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gpssshpzt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gtaizbbuv.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gvapwoeyj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gyoshalvh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/grhpgqdrh.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gjjjntpru.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/grlillcbo.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gznkldwkg.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/ghfuhxymo.sHtML


<!-- 参考信息 -->