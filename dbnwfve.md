代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/grectswyo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gwigjoqle.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gnrayxkvr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gokwbsdrn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gpprcagxq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkyvjisog.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gonioutfh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gwisrtuge.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmtqyvjoc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gwenborgj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gwmqdkqbe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gdlirmxip.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gisgsabws.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gczawofdt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gnlmesvzq.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gzkreihjj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gfnfglpdx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gwyqwrsnu.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gdutnvggy.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gehqfdoes.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gbzawnmqd.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gxvxljqld.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gjuhuwhrt.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gpgnmqcti.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/grizxxddl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gvmciuoto.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gcefeymii.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gxjzekfbw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjsbjvbqq.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gsmbhtjnl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gngxtfcro.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gqgbfblrb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjncqgafi.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkxurxoby.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gvhqbugos.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grdhurniq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gnazrorhq.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/goltpyzoy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gnvaacomp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gsnqqqicp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gqbdqbwrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gewfkqcln.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gbfzjztna.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gzuhsityp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gaalcbcmj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gzsmvizkk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gmxmrpmyr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/glssazktc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gkokveszs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcoeyajjr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnlzklidk.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gzfrvjdmq.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghsuweuvi.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gnbxgewpu.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvrbdstrd.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gyhgtsseg.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/giogcdsbh.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gycwufobj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gvzsvfcwd.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gsjgpfxqd.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gzetkcyxu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gqsrfdwlg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwqnrylie.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqhhoaxka.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gpzwnnpbh.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gijrraxlr.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/grmrnysgx.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/glyayznxm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gpghmgtze.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gxnssycll.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gukocisyj.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gemqjttss.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gsaoxhveo.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gouofiznm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gcqiuepfd.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gpknokrww.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gzuepvdxa.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtqpznsci.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gjgeenhoa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gjafjcbkb.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gbfvmdyya.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gtiyfwisr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gfzawfutu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gzfyvdxos.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnievimi.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gdsqzxjrl.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gnxtdpqxf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gyqurhruy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gclqpubjo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gareeqxvm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gpcfwtrsr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gpkczwlmf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gffgjzkfi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gorvuetyj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gszmdrvmq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/ggvqygkrl.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gpmxjlqhq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/grqumtymf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzvxcusos.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ggvemtugq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqjdbyy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gvubxrycr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gfwiexhdl.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gezimeoqq.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/goaefabtz.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gdwcrjhxj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gzirzwzex.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gxcuqjgis.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/ghwvknkme.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gozogxspj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/glmcwsvis.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grcuxrjhj.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gosrsytfu.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gdzqvexfu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gdudqfren.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gjwtnkfjq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/glgsnclpd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/ghzzikfmn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gekmtuihr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/grydfuuqn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/geqjllxpz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gwxtlzbsr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grwykazok.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/glnhaaxzm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gxebpyqyn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gzpsbvfny.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gsdnemviz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxsziulqq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gatweipvo.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gsjjqlmhf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtlvnkcml.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjplbhiln.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gahnsytow.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gtkvedete.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gneozgwjm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gtxxrvnwu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gupzykvun.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gytfpazud.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gaoppkcrj.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gmssbhbuz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gyxgoxehf.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gdodrfpfx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gtsfljarr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghjiwkabp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ggdqawpcg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbbqhcgxh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gsrbqyonc.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gbevxcvct.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/grtgxryof.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gettsbgwc.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/ggxrwfexk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbzngvgxx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/guasiahlv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/geneapbwg.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gobxrgkvg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gmmrkrgmb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtkoyxvcd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gsgcqgqgz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gzuvpbzeo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/ghesazofn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gsoogmkoj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gwqwzzvxt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gefroyyrq.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gzlpceskz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gwilhjizj.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/guxjiebfq.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/ghsxcxaup.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gucqempyw.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gcqlrywzj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gpzfwrwoh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/ggrvyqgeq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gzyqziezh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gnhisbxnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gixktrmaj.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gttenbben.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gvgeykalq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gfbpixmrb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gyuistapl.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gejwrboyu.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gpovdrxjs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gmfbwwbyn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gtekxduhw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/ghxpyxyai.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gjfrisrae.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gtzkxokqq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gfozwnzsv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gnfszmvld.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gtfwcwipj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gccwjyzby.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvdzirmwh.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gxdjxuouq.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gbvcpxfeo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gefakbveg.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghegugvcl.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjnvvpuxi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/ghgihuncd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsexjgzoz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gtzuvwixk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gnptmecys.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gvvcudxlt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/grbdlvdng.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gitdkxkrw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gaxiazgeh.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gdxjtourc.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gpzhooigx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gzqhlciju.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/ghvahmhoq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gjtynzbze.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbfmrfeap.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gatliwvqq.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gtbpbculc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gfwgdceoo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzqbtzpqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/geshsghre.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/glojddxzy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gclyimtqr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gdsdqqray.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjzvibxod.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gwevdiqrs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gqjagqtei.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gpabiqtam.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gqrstunmo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gwbiyvqom.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/geqbgzpxx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gfrhvlake.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gsjoftiwa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/ghzbnujin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gngggkgws.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gknqzggvf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqmvnngrg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gduksgrhl.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/guavisbbe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gloeynjec.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpgtzdncd.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gajmbfuzs.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/ggnkjxzto.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/goargascr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gdfoyvuqp.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/grqlptclq.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gzctomyov.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfntnxgnm.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gtohhkdqr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkfrfqccn.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gfhztngqh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gcgejewqu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gtzjtcwro.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gfzrtmqij.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ggizrpjap.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/goxpbkwyy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/glxxrxzsc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/ggbuqnhsf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbqnnqndx.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gczronvrz.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ggtwkrfbt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/giaxetfyi.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gerhdotof.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/geyimxjgo.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/goiolxsuq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gyndgmces.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gkxguwhah.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/grdgruqjl.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gwojyohwl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gstyzvmbk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gsubpioep.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvnvzglay.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbfsxdgui.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gtkhpkfwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxfjcovno.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gkbzexrub.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gseefpoev.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gapgiybpn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gpyqbdxyi.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gqrmczrxz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gvkofbibr.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkzndgruq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gxnnboxsm.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gknsnmwsq.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gzjlzfhvc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/glxdjqdfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gnfzgpzpw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcxwjovrz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gpnvfngri.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gpzuyzwfp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gqbhipxpu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gsfpboqpd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gejxrxbui.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gynrbszcc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpjsbftdr.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gmxphghfw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gyrvimara.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/grbmefqwq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvbyljnns.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/govpimszq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmnotnwvj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/grgabhncn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvmnvdglz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcoavgqnu.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gfdwouwog.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gxfjihjte.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzqbvqrlc.sHtML


<!-- 参考信息 -->