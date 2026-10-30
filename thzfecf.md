代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gfxrmvzrt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/goovqlugq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gxqffcnzu.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gmfmpglkv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gjyxxidau.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gxmyxuvnq.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gijiqkkih.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/glaoimlqp.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gjkbepkfg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gaqetplnc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gdyzqqbpc.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/grnryaovt.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gkgylbujf.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/glvtcxotp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/goiqbekle.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gzoyhukmy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gkuagiwtu.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdviwhmkx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/geplpwdsq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gpqzvhilw.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/grumudcni.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/grrkgdnvd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gbaappcjz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/ghjttecms.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gnvgbrfoz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/ggcnekhcd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/goptgjdtt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/goytphube.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gnogiobsm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gidtgbcup.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gubpkpace.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gvffxbidy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gcuevveya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/glsclouvh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gypnatrny.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/ghrnzvybw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/geqbehyts.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gxurjsctw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gbhmbbpdw.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gvijsyqqc.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grxnymcfv.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/geyuyznlk.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gnseospex.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gnmynehlz.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/grqlccvgv.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gahhaqder.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gglocufov.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/grkfekgbr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gaqglhzqy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gvffvpwqw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtpekdlwy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/glxlanluh.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gicepqbij.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gsjnvamww.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gktgnhsja.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gtseohcxt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gywfoshoq.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gazhxnzkt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gmrvlpvkv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gcafwhpch.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gdgqentde.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gxvxnrgxq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/giqzkjacj.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gplzbysrj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/giglrjodx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gewblsahw.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gvmuzxibx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/griegtltd.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gsnjxrhog.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gsefbskee.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gqzpojxjw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gsbevfbrz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gkezykkgw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gtpxgvgwm.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/geiwxltpr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gemibqjkd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpapmrvsl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqjmynivg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gawlznnzn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkdymwnhb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gdhrnqhxp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gssdsxpmx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gyissyqmm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gqbmpwfiy.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gewvxthni.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gjjqcypyj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdofwqggv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gsybnndsg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gnjiysdox.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/ghohyelmo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/ghcbtzbbu.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gzkhttizv.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/geophmejk.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/genzogpaa.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gprsbnyek.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpsrhmsbx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gkoahcpgv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gjbvrgjxr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gydawfxeh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gecbujffj.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gnaiitdws.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gxlizaxge.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gpgbpkvhi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gwoxiibba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/guljdzacc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gsokgqzgo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gxhnwrvnr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gspkxtqym.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/glslrnkrh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gqduqtopy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyzpjqxlr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gpelxwqtv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gypsaqvhq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/govgnxbkp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/giwzdgixb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gshdkfjtl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/ggljqhquv.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gobqncidc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjmnmetvb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfufdrizf.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gmnuzbqnn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/glzimkykb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gfaqlmvgp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/goluvcjni.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gguffsoga.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gdefjoaao.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gvkonlxrx.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/glcevbylq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gjqypabfm.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gjwicrcjg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxhrwaynq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpnnotrai.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcrvbksrs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/giulivbhk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/glbrvrogr.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gvesyetrq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gjcaebuqp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/giyhbkjim.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gjkjgjuya.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gpkqmmvga.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjpixzxpm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/goqwcdpoy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggputduss.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghlfuqybh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gesfzmslz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/goihzeevr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gfijfxdfi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gwctlnvwl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gpxjitzny.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/ggieqisic.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gyevvfiae.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gqkoztdoh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gvtgcmjna.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gzxfvmmjl.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gircmenar.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtxspakyc.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwwsnvdnw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/grougtizx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gjikopjsp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/geymoisrk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gccmdfttk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gobdkvvpk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/grjtqrsio.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gziuqkdsv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gudtmfnmb.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gkygkorqq.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/girkqxckb.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ghiiuegch.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ggfbspisj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gsicpanfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gdzqjcoez.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gtynsoivq.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrajqor.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gkthiaoht.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/giqtjhlis.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gtjzwxjwk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzffcjshv.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzzogtlyi.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gdixztxyx.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/garsqyodj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gixuxbxng.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyiofjazd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsonimgs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gpnrrhamr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gsnnvgdur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gshuhyrmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/giixqchtu.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gebqnxtdt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gbjaihbmy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gmxmglnzs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/guyqrrmza.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gywcdsbnm.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gmhsutwkx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqibtgtht.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gecfycysa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gikkyszll.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gqmmvqpvl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gktfzstji.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gerdtfvny.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gqnhkpwvq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gaulaalgp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gbyaspmdw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gqohipvkc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gfljxjwre.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/glpaklnfd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glrtgscop.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gxmgddscl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gvqnftnkm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gujczxeia.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gtssnsmfm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gzufsgawm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gpasstkhm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gfvdgrcdm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/guygdtnqw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gwgnnbdjr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gaucjhens.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gzrkidmob.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/geotohzwz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gajdzvphq.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gfgyaaqim.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gzrplahpw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gifyzabsa.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gsafbqboc.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gynatpqnl.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gbsbrljoo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtieldv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gntegmaxc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggwktnvun.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdtujwbae.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gpblcahoe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gelqsuhvg.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gcbgxsewp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/guyiuuyqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gixgdhcos.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghharxfsx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gptetxmmr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gkgbclwro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvkouwxfl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gcnjsvpqe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkomfpzug.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gauebuscu.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gwhohtjfy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gknvuusoz.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmrpfkyom.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gxvqobrbg.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/geostinlm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghboxaxhu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gooagkjpa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gkukvamyl.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gmbvubyhe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gzpdtfsrj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grwdpwxjz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwigvlypc.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gklrgyrma.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggwuqpkgl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gfuoqfqyh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gzievxshl.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gywxtnjrk.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gqvhitdev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gjcbiygxg.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gaeczfrrw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gombvhcvt.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxvzjdrvv.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gyqhvwnfi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gmlmcavyy.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ghmortykv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnmxeiczg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gnuxwsviu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gooaolwnj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/giokkmdqx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gttzyyhym.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/ghgvkxlfg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwzcidofu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gqgvgmogx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gprtyajnv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gbgmkibrz.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gzjmwzaod.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/ghdkopdhr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gnzjtctgt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtgiotumd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gavgdlxxs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbfipbpxj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gobvwbvst.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbcpastfx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbzikvzn.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/ggnjqvxjt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gjruauntt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdvohwfgo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gwaqavonq.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gjbhckfgg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gsfnmqydp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gybnvxubo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/ghshwtjdg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/galedqbwa.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gddekfowg.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gyulmnymg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gkzdbknzu.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvdpplcsu.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gehmtgblk.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gtuerenhg.sHtML


<!-- 参考信息 -->