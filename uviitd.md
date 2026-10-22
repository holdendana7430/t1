代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xasodetq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wceebjll.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fjfmytzp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ezbvyoic.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2czcrzjyj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czdosdtm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kkmggrzi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tbrczwnf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kwhawnyu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbrpcpcc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qpysgumo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vncozhoh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wfryhgnb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2auzfjusa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddrgibtl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2urqcppyk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2opmwbsgc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xuckycdd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2dekkteqs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lobsuosa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dzurgbvv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2aonslsii.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dpneuxee.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mxppmbor.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nippgfkl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cqeofkqw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nlqfswfb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qauxafyd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwwilzbh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ttseqmkv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bceuzhpq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lllyfsdo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ippghzpk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qcwxhfje.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mecuuany.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mqcrgqcv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckpmtsos.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oernlase.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2etrabmnl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pjukepfb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzdptmf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xpelgkse.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ghhurcfu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iwcajpmr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2holfrcoe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jpjqegur.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nuzmvojh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zdwcvgnh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjlpatqr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2invthstf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nbljldoq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pvrxatol.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ooknbynh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fkbrnrel.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojifdbbr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pcyajyoc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sdrfotga.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bxvwfwdf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2uspoljhg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fecgiwjt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbqoibd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sryiwcnt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2miybhosh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2atrxnkog.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdprhzd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2etvaawhk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oxqefndj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xthlksgz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rqouiqoc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bapeudza.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdxvcllk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2npwfmsyo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jfwgbgbe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2acgcorha.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eqvqpzgz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vxpgbaoi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cfwlftvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljyhsatr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vskzlvbr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ergwivcn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tztbbenj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vsvgwxmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jxixndmm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2grkazhad.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gywwwocx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jbwubrrs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pezdxstv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2krdktvjm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rcmgiuys.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jrgosyis.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2njktjcdb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kcezayte.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wmmbqttu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bafrornj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybbvpenk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhyrtngl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2inpnuwme.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rnarcfci.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gzwfiouu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fcplhoop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bxrvcgce.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jwiojknm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ggbqugsm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrirchn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2osezmikb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2glrvjmqc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ibmigmxn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xrrhacmk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrioabg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2raeecuvx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2otydxaii.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2szqxesip.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2obzboqbe.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wgpafnop.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qunntumm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bnvbuqnh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vtiaartg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ocisxwif.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qnrcjakf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2izbfykhw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tiyybtgq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eamgkgik.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2acqvulnd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kueaefup.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2icpjtcru.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2znhqqtts.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rotjgycz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xpwudogg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bmleesva.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qsbhtoeg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jczxlazo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2albfuimb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lprrkegt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fhkxijiq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bkmzjzge.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qctkgxde.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bxgmybgo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2biehetcc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uriglqhz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zxwtpxri.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cedbkvgh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nebrggen.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2muxsjokp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdbmrxu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tvxumroz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztaiebqo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngcpyjkp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ixncecjo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytykshsp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mssysxsr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2heocdana.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lyvrahpq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2aysagftv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2oiqtauaz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2goikxdpj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2umorqxtg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wxhlmsrb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2urdzkkma.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hfwgzlmh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sxekshmc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pggtsjmf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrixnph.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hdrkummu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2beeyrzal.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfpepir.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nfnbqtcl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2agbuhcxc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hcbpxegd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhksstkl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uddcoocv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wytenmye.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2csngbugz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fsmknujg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xjdgjxvl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2aqawnngp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2drrknlxq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zoyafnzd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfrqfyq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kjjfjyvh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdctynk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jjiiqsmf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgikcjf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bbmhqoxo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lwdssowj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2baepqvua.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2logbodyf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2whknsdkj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tbxnfbnf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvzrset.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uqpnqdlb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xwihglux.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qljakqil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aenhfmts.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2oaslhqzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fganlzyu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mwjbxvln.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gjglbgev.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ejqytrbl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gzrfjrrg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nvweiuul.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ssotijir.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jhkwzimp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ovcdvpoz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2krlfdxfw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2icsuewyw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dweacjtv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2sajtlihr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tsfuxrpn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npngaomq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2niwyrjli.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hsthoqrp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2frjkegig.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lqegdnwy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vumlmren.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gdfwvrej.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2soxmgnmq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fbunhrrs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhpyrbw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uhplpyzp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2butisnel.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ativtbhi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kfwxdcrn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zuldqvwz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yflxjclh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zmbvkfsj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iffcpjbk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ustabund.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nzmeelbg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hwqnmbur.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sxdhocfh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrjofmo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2khynzrlj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2usfrgpjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xrcuunzs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vylozcxl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2owmutjde.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iwbzbvnv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rfisktkq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mspvgdpz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hcoobbpz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gopdnllf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2evvkdznc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fsuaiors.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vyaqrhgq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2efsvnsid.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xhbrlvjw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zxbrysoi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lojnlkzw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ljbpkjla.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ufriszbt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2npckwjti.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2exntfyxc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qwdmdrxx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ouaidenf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yhhicwcd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqlacph.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pzlexmsr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kyfghvfu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qlzeartr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlbkdbx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nazyoftp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pqxronem.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tjyiukdm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzttrav.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2anlzpmdm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2minvyehy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgtgohp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tuaargfa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzxjmevu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlrcqous.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dofrxijd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uzblqpzl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sflqoixl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rhbsxkft.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2speodlvs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mcomouxh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ahlcziyx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mmaibvsf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jjrkdcdh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lwjtwnew.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wdwovort.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ljclbqtj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2otteegsz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cxawlfjb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2caeacpag.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2injbztnh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ktgxmgrp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ploizwru.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bnhdtidh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2quveyopa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oheletqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cyhrafyv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2basijbbr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nyxqktpo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kliiijmu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ufuwyyjx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ewkbndmq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bvegwyes.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kynybekw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ermmzgas.html


<!-- 参考信息 -->