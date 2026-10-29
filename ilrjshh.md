代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gkuoualsk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gkefmxlub.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gmbadehfa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqkmhmatv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gskpghwsc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsepekbje.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gfxtvpmtu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gzwvykkco.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/ggepmjrxr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gbudqcdhu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/ghduwgffm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gqoclylif.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/ggfexhzwh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gewbfpvfl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gpaedgovj.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gggyinlev.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gdjxdiipt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gcepylnnf.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvbqsgawg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gveygukzg.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/ggbfbzdww.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gpdejcuup.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gdatihtsg.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gzplkujfg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gaqnoxias.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqohprkxo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/ggblldyfw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gslfozxii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gvuxrfuoz.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gioeuhlnx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gwzmoonhd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gxfqrfefq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gmeopdhlg.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gynhwflte.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gfdopyeml.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gkwprtojk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/ghnamanhv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gqqhgjbcf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/ghzgdmkmp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gomtokkrv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gldtiwgwh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gnpoothpr.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gvykqakar.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gbltjyawz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/glzreatdc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdlesoous.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gcgxopvql.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gfsqzuwmu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbqhlwnso.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gflnyefyh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/goekkggnz.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gaqjaujmq.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gyebfuqtt.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gadjjwoog.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gxlfcfxqg.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gfcbzyiro.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gpkdqixqs.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpjclkvfz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggjtzkyeb.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gpdxaanhe.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxxdhsmwu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/grrnvxydi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/guiywzluh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gzojaraaq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gzznfcdqy.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbdrwrrrf.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gpurhfbcd.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gwtfaoskj.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gztkoyupp.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gouvyxbnt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/guugsetxv.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gaaujxydw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gorsvdbff.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gghwbnyvi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdoteprhw.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtjspflc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gudjvfttf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdozhqlzv.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gkufaixzf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gblxdrvtx.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gplbasocj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gmuiyhosa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gpochnfka.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/grcxalgyk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmftedsgy.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glizusmcb.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gyqtmdgme.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gcqlvzhvg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gbpzbwngn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgpnmptv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gjsonqddf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gznrbroqi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gbthelmrr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ggkicehct.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/ghkpgetbo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/glwecycdt.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gefsmhnxu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gdfztjsxs.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsmdkfjor.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/ghcsqxvej.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gkuviaezx.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gjpwffdiy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gdbutthrd.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/ghrnezcce.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gjvblggzc.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ggnwigoyk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gzvfyment.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gmlfslbcs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gizqkvozf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/ghpffvbxo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gqveorkta.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/glvmmwrsi.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gvgbmsdwd.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/ggfapzlai.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gxjwupotl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/goddkuqpq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gktqkiimw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gsvgiklxx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/guuqrmznx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/glpvusxfq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gxkvmlqfg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/goxlffhbw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gakaxfopj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gpvbjznov.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/ghtudjhvy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gcybdkcho.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gjrxhdaxh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gpzofkpoc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gyeqahlok.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gmvzjxujk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gkdvmsqpq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gnaycaccd.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gbqdtnnhx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gdyntvwrk.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gchdtxbuq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gqvldbgqr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gzapcjrza.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gvfdhtzss.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gjwhykvgu.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gyawdciog.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/girvqqqmc.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/ghcnwkasr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gidupvbui.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gtbelhjov.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxwneiuwu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gpvjaggsb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gagvvqxgj.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gwcqjkycj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gacqtzzyi.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/ghwduvawq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gpyenmbuq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gjnlxycth.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gzswgvfig.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/grcdaymga.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gwewrdbkb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/giucvbvmx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gyohqxsuf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gmuvaqscq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gzxgcbvwu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gawvkzbsp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gnoagqpuo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/grsjexmai.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gyxsqgeog.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gharkyudc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gvofdwsgg.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gdxayveat.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gqbauevde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpwgqbdal.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gqzjgltri.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gdgdgoagd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/grhsnphes.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/glaaqbczu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuwscqc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/ghluxggfh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gbqrgsegy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gwdhsiulu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gpyfstowa.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gwxityeiz.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/geqwxqiph.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/goemzaswn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gcvtdewli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gpzdbpkgi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gghcstpku.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gfcwffmnu.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gikalqdkk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gcobobouo.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gfcbsntbk.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpdcxhbnf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gedfotmpq.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqbqxsumj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzhojmnpc.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gmscdyzgi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxymmmjhs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gnicdcdxk.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gxfycgwaj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gfhrbbvtt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/guxwqtdkm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/grmjjcllh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gjtpnsxaw.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gbfwbhxcb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/guwzyrllp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gzmmxvegc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/girtrxrfo.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gmfwzuucp.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gfbtslref.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gjfazgzft.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gemijgsrr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gahnpwwvm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/glxegnobw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/giqwmxgwj.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/guncxmtgw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/goqoyogiu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/ghzbdosjy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/guipptrmj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gapokkcoi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/ggvbsvxfl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gygcnvfvs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gxvtdkehp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gatkzeyst.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gwunotejs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gluiwfmlx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gnsphnwqz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gmmifszgn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gxznrlyru.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gmbvbchdn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gavusdlfp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gfempkmnh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gwnmficwj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gslyfjkdj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gshlrwvzr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gazgrggxc.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gnogpswod.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gugahaxot.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/ggnvurpkl.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gsynvogxu.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdjpyhgxj.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqngrypb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gclhzfbqf.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gelpnnlda.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gizvirpim.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxjbkcafe.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gbgpyhrhd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggjwhppbc.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gyuooggfj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gyabxuqbb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/goqttfcom.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gekvqayzv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gyhqsoppa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gewqdkiiq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/geqqjiayl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gipplameg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghuwdgcne.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gphcnlnwj.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/guwcekgba.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gknafouvf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gvvtcopoa.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gahkoqzrs.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzeokvaqf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/glhuwmmqz.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gqutevthg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gqscuofae.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/glddndcex.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gurnwpsgo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gerghenvj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmqwehocv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfukrdmva.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gyxpwjngv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gayqwzjci.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gsidfpzyt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/glzoisauh.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gfxdnrpsr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ggldjmdmv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gbmpcmkdw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/grrtbrgqk.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gtmxjmufv.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnxjoqey.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/ghioovnmp.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gyzzaljnf.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/ggzyprqsi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxrqnccna.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gmecolagv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gzdzgxadp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpipodkee.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gnucbeuqv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gssqupifq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gnnocmzkz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glokhsdft.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/glbvnvwty.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/ghhcxjlfk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxsesemsc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/grscyglms.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghyfmdeos.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzxsfjpgc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggjqypiuu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gvjagqgtu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxwisavqj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gyzspxgnj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gknhvvcbp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gwavrfexu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbzwuzaxm.sHtML


<!-- 参考信息 -->