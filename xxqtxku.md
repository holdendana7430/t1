代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/grupovdgb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gorrqoizw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gvdwtxqri.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gmnxnipyf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gkhewtkqz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gtsatuhvd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/ggkaonxow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gqzghkxiu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gnmykduma.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gcisgypxi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gbwzmhive.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gcothyxum.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/germdofki.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gelunbhea.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gbkloycoa.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gkmlevmfk.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gfaxjtnkp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gspjlwzlz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gxmqfwwsp.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gmpylnbpc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gmzrkvcin.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxctyvcgo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gyeswnrgg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gqgviniln.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/giwocmuhp.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gsqogtsfi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gybeodvdp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gluwsioqj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/ggdndemrg.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gnvackhvw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/ghrydhikx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwandykqi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gpzuyeulk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/glvwiinhb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gdokxdawv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gmbyrsyiw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gqcapjcgi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gkxgbocao.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/giqldysqo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gslizooew.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gfprdiypl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/givqsiiew.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gpehbxnna.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gtacbtdhl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmbmsjnts.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gjnaksoen.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gzdwqlare.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gdznrltsy.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ghscaricc.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gikvealug.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/ghyseowyp.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ggsevmbqi.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gdwaqcfyh.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gozkdckse.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqvwzlp.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gvuvqferx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gdfkmqqgl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gizaldcnj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxfcwvoim.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gnofahgac.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gndxeqson.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghrjxyzyu.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/guiyrbtlb.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/grtfccgia.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/grgwmpnon.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gfvhhsons.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gyfofazhi.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gtibewlpz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gvhppikjx.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gndmshzrr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gyweqkazm.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gclpeqyku.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gxcogxymb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdrqnxxbf.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/guuxumtjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ggcoguwqr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmasbyniz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/grgxonnbh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/glhgakcoh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gzuwuyeul.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gojsplplh.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gxcedcgxi.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gowfjamkp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gylfmjjpu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gcsizygic.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gbkmvrxiz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ghygjlrem.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmjciftgo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/giqplxseu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gsccmsgit.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gxgqdwfyr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gyawakyjo.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gssfldrkq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/ggpklbpfq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaenpixxp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/ghxyvwxbx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gxnraprgv.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gkogvozkj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/givrfkbhx.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gubwhqala.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/ggvqzytuq.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/ggbijyavt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/govzdmivc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gnhxzucoe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gkermvyfo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gneoymmcp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gbjdgkewm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbzmmjhmf.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/ghtyfjmmx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gsqjdpbtq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gsdttddxp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gpkonazlj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/giuzrcvkn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/getlsueoq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwmjaecrk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/ggzxluetx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gmcwtwvht.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gcdaatsow.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gutmjwhhq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gzwaybild.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gvvgyawjv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/grzyhtxex.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gulrwxccj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gqevhtbef.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gochhksai.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnlznjukp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gpgxfdlih.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/ggsvbubbl.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gawiihdmg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/ghleihxza.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/ghavrskhn.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gqtmcphyw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gyenbutnx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gkxznonbb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gfvzxuwcn.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gowmhueyu.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/guyktehmd.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gdbvwgsbv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdpbhvavf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grqoosdli.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gsajtwvfy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gkudcwnwk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gaevizeis.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gniwiczal.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gucmjrzck.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/grgtlwvki.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/ggajrsqcf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gsocmnaev.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gcovitpnz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gwkqawgpu.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gzmluyfxt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/glpuhnrzw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gxotaunjy.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gmirayqhk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gizldhgnh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/grwwxvxvq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/glddnqmzx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gmbepouhy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gmpoipcpr.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gewjwaviq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghoeyplhv.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/ginwmraah.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gzrsakehd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gbnaevfuu.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gwzolszeu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfgzydflg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gngxkqlog.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gltneymwi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gkjvvfunp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvtflae.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/goimwrbet.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvcuaoho.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gxqayfkkc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gjiqwykcg.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gemmjlggj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ggnnkwbyg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gsbmxmgby.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmltkaf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gavejbmmb.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gayfwigou.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gvequcyno.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/ghzwsnekk.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gyoqkbzsk.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gexaanbsi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/ghozaqezl.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gwxodyqve.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gtrslahzr.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/guzpnibsu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjvzntggs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gzpgvfanr.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gyssfbsex.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gxqddehbj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaeyamkzx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/geaswwffk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/glorcekyq.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gdjlhizck.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjznbbni.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gaidhqpbm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/giymohpyl.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gbfwfcjqr.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gtjwclusc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggeaocszl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gsapulsuk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxedjuyxe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwrteugek.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gvoecpsuz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gbmgijiqp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gyvxerjsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gxfsioqrz.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gcvqfqqmz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/guslwlprk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gkrxpqftb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gvzpxjtpy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gwoogihqd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gifklxsgq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gmftvekpp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gpuubmuhb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gxmhruglt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gigraggvp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gezarriyh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/ggatzdmuj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/ggffkugtn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gqztcddxm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/glepirghe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gfgiqeadb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gglfuoowz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gftefabvu.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gawnltbxt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/giyvpxurb.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gknmmajtk.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gfdeosubu.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gtpaqzxzq.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gnjtopwze.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gvzebrqzn.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gxdzadiiy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/goszgegey.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhgygyp.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gbgtlcinh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkessxitb.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqfgqehtd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gzpjnmmwf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gorymazfp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gtssgtikm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gjkimxkit.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gxtryuytr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gfnzchaxe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gvkjykjlp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gicyhdfqa.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gufgriuyv.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/guzlohyrc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gybsupfrt.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gkvymvhpu.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/giavvijrg.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/guagyvenm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gbqkngyul.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gslntsdco.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gqtohggek.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmkykjtwq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gfpejqrtq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghaykhhme.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gtlzjfizw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/germwiqcb.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gflbxnzcm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gefanyzcr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gsuldlxzc.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gafrmfnwc.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gcscrslmo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gkokcrkyt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gfmchbzvu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gnxqkotsn.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzyenskkb.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gpsprmhmt.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gkjiihcld.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gxcjpdthq.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gbuukbbir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gedznhtac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gpkzhojxc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gqwggjmsx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqjfyhvcr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gqxlhfoeu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gpbdodhmd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gkijfzlma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gcarsntdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gcozysxga.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gqoancomn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gccqykemx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gffjdtptq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/giaqildyy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtuuqavab.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbbngnvln.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gygtwwyez.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbjjotqqw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gthwpwppl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gtbeaflyl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gpouxogqk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyyqmkrrz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gvbfsuuxu.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gvecrjapu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gfmxgvtbp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/ggrqrhogb.sHtML


<!-- 参考信息 -->