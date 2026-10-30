代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gjdxfmbrb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjlkswokm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/guimaznmo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/guqzwzecf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gyuzakebc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gcmdwoajs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gjjcozhzi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/goxveumyq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gxwasgyno.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gvhptzway.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gzgzxeqyz.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gemjjqbsh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gpxcyuksm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gwupxqlkq.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gcbcgzaxv.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gqbdttznr.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gtidzuhdy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gtxcwfwrm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gbjuaefgw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqsswlst.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gmibzdpur.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gpujvpcgq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gbvbxrmki.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gxwkdjgiu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpuytuzub.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gytugmtum.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gapqsmdky.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gmdwhrlfp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gdwofgvqh.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gpmgpjxes.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gfjlllkis.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gwcqdkmxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gpbpullgx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gmotayzbc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gbhimilvu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gcsvsbwot.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/ghihrzbsl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gigtnredd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gfrlxgzxw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gmdkaohhl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gcmsuabcs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gfwffvvgg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gxlrbnvvu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gzcfgavxq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gvobktjbr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gjzcqvzwb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gsbmgftiw.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gnstyhmjz.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfbqpaays.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gissuheqv.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/garwjoudh.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gutusxgfh.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gnexmmjkw.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gocawjrhn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gqcrvlqnx.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/ghutjudxw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/guivuscxs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gzihumixq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/grkfcbmxs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gvskznmst.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gcujhugyh.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/grbqbabet.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gsuhpaoph.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gsxnimour.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gfznmmoyr.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/garkwnoru.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gsmkgmrce.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gkkmwrhde.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gidgwehbx.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gekduoetp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcebgorxa.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gxepfmtba.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gfaympagy.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gpqgcgmui.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gcyvrqqov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ggvclzlen.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gswwlwvys.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gqkwdiyzu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gbwmawqok.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gthawiddr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtusjgagx.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gvnbuggkz.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gjcjjmnmn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gkridtiaz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/guourohnh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gnlkxisrr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gfoxtqusy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gkrobufnn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/grsmgrohk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/glelfwiit.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gctsuianu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gkmpmpasn.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/geagbumxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gneiouitb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/grynyapiv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/grgxqesia.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gctviiovj.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gvumgfjpg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtieleyus.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gfnhupcab.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gaumdratq.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gxiibshqp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gnzwkapea.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/ggixbjczr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfwarmrwz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gayqpaezb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gzivdgtbt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gippdoqxi.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gnyobhwnf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gymmnkejb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gqbeefjaw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/ghhttokgx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gvvvxjszr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gqpjpoqmh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gcuwbjugy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gixuywppv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gwovezdvr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gwvbdtvrq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnwtkewax.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gobmgrlss.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfluunqje.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvqwjqsin.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gjxowgxpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gnejefmmr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpidjddvv.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gadjfyyvo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gtwwrbyhd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gzgmghawn.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/ghgogknev.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gowjefnrj.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gzcutbkbz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gwicijeck.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqqottnvy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/ghucabezu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gzibksrek.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gwmcetwrp.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/geqmaedze.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/geeblpinz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyflyukvh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmtldoqys.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gvjmqeryc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ghckffubs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gmrzygtul.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gczdstasn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gakhmjlib.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gmewtgqjo.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/ggymjzwik.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gloesaezp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gbpbwprbw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gozgyhxbf.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gnlgtmrny.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gifjkfpry.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/geoozwcci.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gzjaupnfh.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gahplcalw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gkexgkbbi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gaxxidluj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/goztvnimg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gyqwutnme.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gddiywtkl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gyjbatiyb.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/grywmwtgg.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gwrnkkfdp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gzytqmltk.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gkeltxgjd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/goruytcfy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/glsrnyogw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gdtddihne.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gftkaikoc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gmvvatkdy.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gldycldng.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gbimvhjqz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gsmblchfe.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gmshjlaiv.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gpklcwzey.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gkdqepzra.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqtzhshfk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gjdadcjnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/golwenklt.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gjfgoqkdt.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gmqvcigmk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gkzsvlfjt.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gvhcuxazu.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/guamshzdt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gwnlyizva.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glnzrqfut.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gfbjvfvxf.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/grynjpuuh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbvtuljvr.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtkiyycbw.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gcdqgosqi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gebhwpixo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzeqcklwz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/galbfuudb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gveigvmoj.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gzjpbfpni.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gkjigugiy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghwebstly.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/ghkhmvjyi.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gedgqjgdb.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gvkrdraea.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/geqwyxjhl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gbqambeij.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gexhfydif.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gozxtxrmb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gyhbaqghh.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gzzcsnhpx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/ganvlowex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gftwohklp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gktpdnfqi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gcxyapmfu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gqcgsmrpn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gamltnupp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gygoarnmw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gupaajqpu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gpocavwlv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gxltkcgdo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gdxbbagci.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gzajmrkfe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gfauykbkl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gskonkpex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gyrwgnadt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gcnqmvert.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/guijfhier.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gobztiwzj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/grkaccyhm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gggqwytxj.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gwmjclqyn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxjbpdxwm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gyfklinrq.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnpytvnpj.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/grxdkwynk.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gwrssljme.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gpbmuhmhb.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gehelprac.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ggnfdjmno.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzrvbcexm.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/giaecfabn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gefklkbmz.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfbgamxrf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gtmeiyetl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gdsdwwpgn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gnkvedovu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpkcwwxqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gehkzobno.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/ggnpwoglg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gjexeycvy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gyvlbildx.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/ggrbvqbjg.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gjqbfzwpy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gtothfkhb.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/giejltufd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghsudihun.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbmurvvev.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gfryoxpwt.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gdlgpcxzn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gqnlnjqbh.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ghuwipkbp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gibfbndch.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfljtjnbn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbkffhduh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gewgvaszp.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/goysgdsjm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gnyvakrvb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gabkrovmb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gtgktkqbf.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gtlhxkgvz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gaizcicmu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/geupdtvbj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gniyhzafl.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzxgxqwul.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gnqflvhil.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gvclfuckc.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gostvwqyx.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gbyfaruxr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gucxdompc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/geehxbhxe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gsplvfuwb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gdhhwldkh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/ghdyxcceq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gqbugjotj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gtsvydrjr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkgvbump.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gujzqgein.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gzjcdexso.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ggvzkygyq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gieruqnkv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxkfshlzy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/geqnyjprm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpkmjumgm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gxxouepzs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbobtbtbo.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glckcuoom.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gbzshvdkt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gnepkmvex.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gnbeshofo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gazndrmqm.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/guiuakzuw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/grgymzrhn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gzzowxtaz.sHtML


<!-- 参考信息 -->