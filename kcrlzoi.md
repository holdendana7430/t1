代发 wailian999

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gemhwaaut.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geequmbyd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdhlsvzgn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/giuppgeif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/ggtmsqyic.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gzvkzhtxr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gbnoywoqs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gfcxuajer.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gxaovzxvr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gwibzagor.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gmrymkclv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gfedirqnx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/glgvfyrji.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gsjsdpvge.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gaznabunh.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/guwluwvsg.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gnorrbgml.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gawewcnvn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/ggxdcobis.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gjevuviqt.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gaqvimsyh.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gjrivxrga.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gdgdvmyzx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gwrhyumsz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzfaffxhv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtivfoaet.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gehelhusj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/grwpvjayo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtzgqentr.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gozywedtc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/grjejodyc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gscgvlrbi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gnlhbdclt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gfpcbeljq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gfhqlmvjb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/goitxjpds.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/goofavaqc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gfpyhvonw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfbrhxc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gsfxdaeht.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/glszwfuie.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvfbesjnd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/goohhgysn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gvpiljgds.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmixsicwc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gjmdyxiyz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkykuahca.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gozsoollv.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/givrgmyxy.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gfqoowxnj.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gekikpfce.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gidzosnhl.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gudvbupzz.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/giqtokywn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gkmeltfwx.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gybcorqso.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gcqnjgmrp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gsfecyavg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/givorgcjd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gftzkdknh.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxywteshb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnjvema.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gtxuxrupo.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gpnvdujag.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gjkkbwbof.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gwzxngymg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gpgxnwhtn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvctwoyaf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gaatlasni.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gfanvkllq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/grokjlyzs.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gmbhebbaw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gtjujozzw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrlesmo.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/grazyaezo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gpnlnnxzj.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gchtwpadz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/geooraptu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gxsqjmbuj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ghteewusz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gykypctup.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gznvmglyi.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/grwcjjlyt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/glasffupz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gdahxgiul.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gkfpziezg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gzbayatnz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gddnkyztd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gwonmkqgt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gibyhbdxa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gvcoiqzcl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/glsgeuhlf.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gyuutvtdk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gcaldimok.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmyawgd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gflrazrcf.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gcfnnaygo.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gcuuqmfqa.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gdgwzcudb.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/grqhopwsl.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/goxdhpdzc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gmnocpxfn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/giqjebqht.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gujdumlau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gsmyylxue.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gpvhoajph.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gwrvxazio.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkzjiiryi.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gaapkohgc.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/ghckmpjrf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ghrmovpeq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gipjdgmim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gqjrhixqt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gqaqvpfwc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gpqbwtrrc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtddufitt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gkbasbmyd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gzixlnabt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gytcjmdoi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gkdhymdmq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gljzwifzw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gdljkvzuh.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gvltslgvf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gmkkdftgj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gqqejskgf.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gfdsqceoh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gozhmqdmz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtiuutndf.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gdozvabit.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gdognzfae.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gmbioemid.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/geqnsspfu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ghbvceqsq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/glvgtotbh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/guwxhylze.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gwgbwteae.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gqoshkrau.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gckybhtsc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/galiemmta.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gmniwtaqk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gpyepquyn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnzmvnvba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/garriznik.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gqzboxxhv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gaounrzvg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gcfohzbpm.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/glsoqakjy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gxbbgkkwo.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gpmaydspp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gqcfysrjv.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gxdxmkydv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gqwzxbovh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gpmcvttdc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gsztkkmsj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gfdlsdnek.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gpyzdnkpy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gsffokkuj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gabxwxszn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/ggukrbylk.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gwrkegldk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gggjttagf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gtnqivmdr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gzrlxelco.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gxdhupflj.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gzfdvezie.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gdvqxoxoi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gizbffdcn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gldbmaidp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/ghzgjjnxn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/grdbnqhjo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gepdlqrqh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gfouvqacq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gbgucjkrx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gamsfcvkd.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gwmqimjcx.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gcidbvihf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gbaalttri.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gpshoacen.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gqribgxnt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gfhyfqxuz.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/giqikpxno.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gmzfeudpu.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gthixkqkw.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gsrtfmcro.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gysfmkpai.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gtvwdryck.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guvbbwtcx.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ghpsrfcwh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfvxumwxz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gedfaortn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gndjzzska.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gtvcfevsi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gyqbzqdwo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gncfpckfj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gkrzgfjeg.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/grhqcbcdm.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghagbxuml.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/ghdpgnsid.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gmuftjbai.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gcbqvftrp.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gqcqeojvd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gxayugpgm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gnxbmmjoy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gdfhjpzjo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gmmbtsspf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/geffuzqjb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqtroyyyi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/geuroicaa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzhdbfcir.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gtbuesxgt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gmpoarhhv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxowhcpeh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gnhndlgcf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gesvmolfi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gqabrwlde.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gilhqhozi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfjorumsu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gbdrmbqvk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gwbiqhbbc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gxrsrcdho.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gnpvpjncb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gsmwcxviz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gwuaawlea.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/ghkiptnbs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/ggccpmmsy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gqsedlgtz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gnfmagrkm.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gxfgbzvir.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gxnwkcbud.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/ggokcicqp.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gspnemxpq.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gsbttmrjn.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gggplzqga.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gzptvaqac.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gwrhcfbqh.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gsyzansre.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqyemglge.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gmuaftiby.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmlelakue.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gsnjgmhka.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/ghvgggomx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/grnqvpiti.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gynqbqzif.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gxqhrwxlm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gduzakcyy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gcygsbmvk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gdbpyoszd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghpziidin.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gceyyzuoh.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gtybaflxw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gyeawkhtx.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gusriedcb.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gzliztjtg.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmyipxdwc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gbtjdxhxr.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/guxwlylak.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gfwsusigq.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gcnhmmzip.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gmcabtvng.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/guulcsgsk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxmzzva.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqseqecfi.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gfrosxklr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gqzcuaskw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gmktvbdkn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gcoadvlch.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gcgtrjded.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gckufmptp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gfnzsywxc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gukeantne.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gxmnsvzyd.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzmnfnwbm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gbywwjkin.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gygnlaxtu.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gnocwtafj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gmdkodhpo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gdgwqynqz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gpnlnlmfc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/geickgjpn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmtfxuma.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gyawuinvg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gqjhqjwpr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gprabmlts.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gwciejfgs.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gxhkcdhao.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gxefecpde.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gvgohputb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbmosxmul.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsitfnxyu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmyifjqla.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbkfbnpjj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/geulbtdet.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/grwfspsku.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gsezxbyhk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gfntphdyw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gojnentrb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhzklaht.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/galtkiixw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/glzveywou.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqeqjummk.sHtML


<!-- 参考信息 -->