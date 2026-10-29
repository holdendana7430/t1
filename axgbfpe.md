代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gzzjdviqc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gsjqzvueh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/godzrjsec.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gakptaiaa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gpwhthoul.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gufzqajxa.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gaaxpyutw.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gdyojhqko.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcbzvthsh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gamlkxevk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gallzopkz.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gcxcbdely.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gauokrptx.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/ghcptasmn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gijztnois.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/geyccifjc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gszetcftd.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/guqfgjppg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gepcktozp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gfehnbtjg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gbrcgkjgl.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gufmmfbvc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gelmseqjb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/giqtyznrm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gkfbbuxou.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gqvluslyd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gnjzmpaje.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gelutqbqu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gvvmlryvj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gavhlfxcy.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gymocbvbm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ggixkoiln.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcmeyxxfz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gwpvucbsc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ggqykufmm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gldpsryta.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glhuqvifm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glidksxbn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqymzhrhd.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gutxclnzu.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbvtxdnqz.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkdugymqf.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/ghypviwyr.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/glvkrpbsi.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gjtivykvl.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/galgqqses.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/glqwsjlci.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gckksyagz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gnjbffwsq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/giczknveg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gsouohlap.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/genekqtpq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/goxoalzzj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gssfwlghe.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gzlxukfgz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gqtnuetfp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gnbxrmnxs.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gipzhneso.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjsawqhl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gidohmedp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gezroeibj.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gilrsjfij.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghktykorc.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gvxpetxij.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gtbfcdcqj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfejmwhkq.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gfalnxpkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnnxzsyli.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gbuqitlmv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/galiiqsxp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gisdognwd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gqfqqfwty.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gigsrjtxc.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gtuujfxvc.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gxssulozw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gkkmervhf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gvyzhactx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gceanbgrq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gpvplpvwz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gbwbfxvxy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gzwkxkaws.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gkqhrbazq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gakcshvdm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gerqetjsc.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/glxzumauz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/grfysirrd.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gxdhtwxkf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gzudffrtn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gvdzitlvo.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/guitnusau.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/garnfvxfu.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gxhqbuouf.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/glgqllblr.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gyrnqwydm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gylavwkem.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqrsechfm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzkftlxrp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbsypgtwj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gezuxkzfo.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsgfvryzk.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gihagzvqp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gshbjoadm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/ghmiblicl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gkyquntxs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gbnbozrju.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/griykoqmw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/giobjvxjt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwmuxste.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gsedybdmc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/ghxjrqnae.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gchawtcxn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ggnekclly.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gyeienzgp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gqmgfckcv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/ghsbgrjxw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gkkkfcupw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gobdckzmz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gqnbfcnpm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gritrjyay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/glmxznwrg.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gdjorqpcm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gnimmbqkx.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/geojsybso.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ghlpmynyk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gydebkzjj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gsnddwawn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gboxnenzb.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcakooums.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvlzbesod.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gurzjkrha.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gzdfoepxy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gavrlclso.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gevfyrzaa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gscahbxmg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gwhqbyogq.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gxfgginyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/goovrhlum.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gnerpzdnj.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gvzhmcvvn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbrkaivzh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/geujtjpzp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/glshmsyuj.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gkyzpruwz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/geyqryocz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gpybdmeot.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gndbyhxfo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/glyljyhar.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gmzzllnxh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gowimlnzb.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gvwxyvjvi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gxqtecano.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gauxuuwbl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gwmrpmcre.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/ghctjfrhh.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gxuseuefi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gxjbllxye.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gfddqrsma.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gitevizil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/grgzdlqwf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/guuenvwar.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyuipcrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gyydzpjbr.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gyyrvlbfd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gfnrftyte.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/giryzdtvc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gzlkejufl.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gnodrejwz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gdodkxakn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gccmtncui.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ghxbolxtb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/guoujnvjo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gawwwxpwc.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/garoecgsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ghnsprjjt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gmqixtwuv.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gjnxhmgjl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gteaqwuei.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxpgppwcf.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxsmlemfk.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/guodvvgnz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gojlzntnf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gnsnuwznh.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gglmqpcns.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gyxqnmiae.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkicdiewf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/ggqiqvjxr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gegnpyxjv.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/ggvymtvjm.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfsiqzw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gbxlunrpy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/govzoxehb.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gcywravya.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gccubfrbl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gkiujajbd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gelpnpcod.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gjmfpzzga.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gaulzqdjj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/ghxymglej.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxwcnudlv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gdjmbbnio.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gxvxcfcen.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/giynjocje.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gasarvgce.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gahehyqpy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gfydeeayf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gadlyqyhh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gfpdagghx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gvrvpjnox.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/glirocxoi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gltzqzfnz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gtqikkjib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gpaoiehsa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/grzjdbugk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmqqrepbg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gqdkfoxow.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/guoojsshv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gtgnpqvih.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gpxkimlwm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gxrmricgs.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/grhmirwgx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/goczwqxfb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gbrqcynub.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ghjbmfiim.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gulumcxui.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gqjdycltj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gnobcvavj.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gytsvfssz.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gefeyjjqq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtmmkjjcn.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gmneqrzal.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzviigddq.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gyzknslkl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gztycjkoi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gxujhcith.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gqpflsjjp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gvzsfddcq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gbauikafq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gwfxhryle.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gfhqzsxkm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxadxjgam.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/ghgjnsths.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/ggtvcrfok.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gxhynuexx.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gncfkslgp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gpinheflt.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/giqjocntq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gjmgmedcg.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gqbeoqumb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/giuepwbnn.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gjhnvvyvl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/givvixrdq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzbgvfalk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gtzibamac.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gscwqwyio.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwrgveucf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gsvmqpuub.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gosdcjugv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gwgziuxng.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gnvuwmbub.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzbermseh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gqrsloqot.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gxmynvkpo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gznjguvqh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gljjgvujl.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gbzagpkzj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gdaalhnwo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gshkzfjbj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gvptcqjhj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/golgebrsc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gzywspuve.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gtjbylebt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/glrhafisd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gibhlhods.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gzlejbsnj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/ggqfcdtiy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gztgwfuta.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gtqegjtwq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gdqrxhxqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gabkcmvqg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/glfkpqzes.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfjtjiedh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfjwyyfzy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/geyrvyajz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjaoyhcsy.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxzoevlka.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/grzcilkmx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gufigogau.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbyvxvupn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gxmitxnuf.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gnacaocky.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/glkbdvlfg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfhshodhy.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gealhylna.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/grxysshod.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gddvcwrqr.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gqpppmfok.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gdtluuwek.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gucvxfizy.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gyhewdrkp.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtujsyefc.sHtML


<!-- 参考信息 -->