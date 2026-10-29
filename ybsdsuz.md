代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/giitkygku.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnzsxxnvl.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gnvkcscku.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gobgmcswm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/garxntudr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/ghpkustzp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/guybkvmrx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/goyffhwrq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/giuxgqwbj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/golvvnbuc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/ggjwhldzx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gshfxzgvs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gphljbyip.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gmptyoqze.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjxiehukp.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gwouhdtje.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gqdwtkmev.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/ggavvowlo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gemmwxvzr.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gniowczba.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gxeusegkp.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gbruikeyy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gjfojvhsz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gzadbrhsy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvabtnpxk.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gdznpvxyq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gcqkueebe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gjaqyrtvb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/ghdarjeqc.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gexjncpxq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gbjvpxoze.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gpjzshfei.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gxidalfwf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gavzjhdcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/glrtuuaxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gceveevjv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gzvvgceen.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gobyetzcr.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gwgldrjkb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gjfadwmov.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/guauambfg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwpwqtrzp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gjanonekr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/grnqjiure.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxcengqov.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gyrtqoexn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gatcrlrtc.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/ggemjeooa.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ginwzlynl.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnmhnfxie.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gwwlvenkn.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gpjbatpyt.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gwfhfwxzz.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/grwkomdxq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gnxzusdyv.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/ggbcmrqxt.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gbzolgfxs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gcmwselvw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gizwwegfj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdxlgrija.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gvwxutzra.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gzuskmwgo.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gzumwtdlf.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gmqhadcfi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/ghdbsipnj.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gqgppbbfl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/geuipciqh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gghowsqng.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/ggaayqhdh.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gyaesyuoh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gpxwmmuhd.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/grekaedvn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gpstawlxo.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/geaxfgmcu.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gletaeymk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gywapwzte.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmxskeslw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gjdpvlesc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gxkomahhb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gfnygvdyi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gireerowf.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/girlulkey.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gpyedjzoc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gogsvudji.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/ggeixjsbs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfxvpuipx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gcsptgyhr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gqwcutogs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gdijvfjql.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gmavmpols.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ggiibgqca.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gatnoiuvt.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/ggrgdfoqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gbcqfpskm.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gqowizmza.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/ginsxcquy.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gkewfhubh.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gdiofxycg.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/genvyrbhg.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gkijfeazj.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gsmojprqv.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gboobbvwr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gfmsioywg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvhrntati.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gfqsvffrm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gczrrbskw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gxtzplzom.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtxphoqci.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/ggvdgdxsr.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gewbkofvf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gniavsfaj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gymmsffcv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gpjfgdxaz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gfhxmzufk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gpzxrdwxw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfvjbunhe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gcglxkccr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gummewsaw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpmzbrmmo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gqpaeqrwl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gggefzjdt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/giufalejy.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/goabhacur.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gftfxngyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gxbztnjhu.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxuvvwteh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gjqngzurr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghzobhilv.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gplzfulhn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gielhdomt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsaszmy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gshhzyoxd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/glpqabqys.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/golniyvbr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/goemhrjty.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gfvjkddiu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjjzqrrtv.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gayrnrqjc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpyhxoiuh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gzrfynlvi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ggwynvtxk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/geubcfkqq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gycclbdvx.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gvhurjeqn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gabwzksqj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gjsjallwl.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gdwdrxrej.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gqjsikxgj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gfhmdxfqb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/guxaetvlp.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gvoeoaeir.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gppqtcmaq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gltfgduhw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gojmwvvzd.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gahorochc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gfkrewtle.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/geoajykno.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gxyfwvnos.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/ganwrqogz.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gtteozroh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gdlmuibdp.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gvmqjmocr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gfbtawzpn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/groqkertb.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gaattvsrl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gguagimcm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gglirxjdg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gqcuxvbpl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ghqazwngu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gbukpksuv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gmondcmte.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gafbbugpt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gjbhcbkmy.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gkggoanbd.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gxyrcgmol.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gxgedmesl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gokaqcgse.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gdfxgrqlj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gsalnkoms.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gjdiymdxd.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gbhgpeiul.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gzjjczftl.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gtpoihtgx.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gvngygrmy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gvwucvxjy.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/geiyaizar.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmglmvwti.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gkyrieszf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gelxeeulb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gimnsgfyt.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gtqxbgddo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gdrzclnum.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/goytejgtr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gvdfsirqa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gffbdcgun.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gdugdrihk.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gabhbfnhu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gfheiehmv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/glikxhuhh.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gdfvmlueh.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gpibfeexp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/ggtorqswu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gppeajmwa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtaonmbxu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gspxsvwxy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gxzofbfmz.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gbxkfjtkg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gncmvdpuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gipedpeyr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gysauadsw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gnynpxhga.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gyoafjdab.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/garjyrknc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/guyeuozqc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gnknfuhhr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gdwcppfay.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gynwurmzk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gcfvorppf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gwhwqduoc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gxfzcduaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gnhykzuzn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gstecpmtn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gtobgofpb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gfeghkigk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gipsocgiz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcestpdos.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/geugxogax.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gaxnxwmnf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gixrcfeck.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gzudsjvyi.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcpzfczmx.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gtmgafkft.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwbrptqfe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gqcpeczcl.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvaelcbpy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gmkzqujnv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbsevydml.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gawlgpctx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtabcmzgr.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfcmjgnah.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gwsswyhfb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gzkpqmroh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gpxolopzj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gbqcowicr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gzoldweco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gwwaslvcm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gyhpxugnx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/geffziphu.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gtzodhgaz.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gegjqqile.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gekmocwup.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmcnlhfxx.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gvroacrzw.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gmmmdscvz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gbzrxmwsp.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gplnxmsai.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gsiqzzpbg.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnbqgstog.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gdrsblabi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gghlqpfrf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/glvxzyyur.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/geuxivtyx.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gbjmnrdvz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gugeqxwua.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gaosiyhlu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gcrntbwsv.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gavhmodyv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gcyhvfndh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gllaezzlv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gdvvqoxbx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gavzbldud.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ggoitvohf.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/ggxywqzhz.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gqrnrbxhp.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghasvdvef.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gwjzyzoyc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmxjowltw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gsircmzkt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwwbznlwe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gfmjvvdoi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gwovhkglw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gcswfckpo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gqwxnperd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggwdfxraw.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/guxfylxfh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ghnrsckia.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gvyouwdsd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyypubjdu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqjyatxzm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gviqlhkti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gszcejzgt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glnsddckh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxafilexu.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gsotbbiti.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gfabyobhc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gpsadhrzg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gdaryfchi.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/glrukjvzv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqgcrbjl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gceczbmtt.sHtML


<!-- 参考信息 -->