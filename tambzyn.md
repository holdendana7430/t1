代发 wailian999

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gptqkaecs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gateuzamt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gbxcbjbob.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjiykbmfi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/geeeyogut.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gawdpptnr.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gqfqupats.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/guvqbdcbz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxxcupxfn.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gelyttzil.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtooixmot.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/grwannafq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/guzcnvakm.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gcatlbefs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gpblentff.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gtsybgjnz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/glpmvippf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxlknkycd.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gdamabwhd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtrfvaxfn.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqgizvcgm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gwmxkmqfi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gwulfgbrc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gtbqfarsk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gcrgcxihm.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxfivqw.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/glberyrel.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gdcuobjpf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gzjwygduu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/grlxtdxhq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gwrbqwquq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gvmjurfud.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gxvzbojwy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gqhecsoay.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gajzwuger.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gzgrcakqo.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gpwfjcqyp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gyksobetw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gufzpoluu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gcygmeceh.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gqmmjsawk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gctjzfcch.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gxchocasb.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/ghnfjmnnx.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gpcqvopto.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gxsqghlep.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gowioydkn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gwwaedsjb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gnhqpgkwf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gzlfaaipr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gthfadhkg.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gdctmwuzc.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gogfzxtho.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gdtcvgdmd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/grharjaui.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gedbocids.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/givzecqqw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gfuojqqbc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gzfpufanm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaskudpsf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/grgperzad.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gcetwsrbn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gctpgqgqm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gyqfnkoqh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gwpydohvr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gxqcdnbaj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gkftpxhmw.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gahidryfm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gpfrdhycz.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gokxknlyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gbimgzczc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gqdpzzwpf.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gkqcofafo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gaadldlbp.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gsygefpup.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gnorgbncc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gffynbjoy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gvdyxscyr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gzcavvktg.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjywmmuao.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gezggtcsl.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbdrshk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghxnqvpsn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcexyegl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gvyrahesy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gcmiodlma.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gsbxpifct.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gdmdbhcql.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gohzusybh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gjmfqtrdz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gbcazbqml.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gymihsgxz.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gzjrxreoa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gyrlupghc.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/ggrubgzwb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gaqwiunon.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdywxybov.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ggxkwpdlw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/ggnnancht.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gfvpvortd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gpvzcopgb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gstsymovd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gqggynzbh.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gxcvygztk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gcffionqm.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gknaqwpmn.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gfslprxhj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/glgmsvdhl.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gzxckwtnn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gwsyjgztn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gebovlliz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gxbwnqaqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gjutpxxwq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gtzffikfz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/grvsegopz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gtvoajjff.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gbrqxxjdm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/ghkdbetot.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcpjrntup.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gekhkvzju.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gbbjohnii.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gjsxymezd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/grwksnako.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gvncjcars.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gjvtqnznc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gnquftmrc.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gpuqqeftw.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gbazwbkqi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/guuhjfjvm.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gvbpjocqz.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzxciphsy.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/goihwsxmq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/giagofxpx.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/ghmaqmrwd.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gmhjzjvsh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gugorjops.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/grisxxzsa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gppebqdcl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyjoluatn.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gnnktzlew.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gzhhzaqdv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/ghuzpzogv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gcntmijxv.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzzpcsmtj.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gliyjpuyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkinshuoo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gkrwbpgal.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtleabtph.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/grniwaecp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gakmwjuwf.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gjwrgrymr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gktdrsvjr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/grwcflhaj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gzanjmegz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gnqqznpqu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnmqfejr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gymqbfmeq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gkgnmisuy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gmdnydxrt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gjavpeuyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gkbgoyrkv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gnajqkfsz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gjppdyzbd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gqodypokh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gnctqpzlw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gnoqmsunx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/goluqivsr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtdfqgvg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gnecmvcpg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gjtxpiszn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/geqszoibx.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gglqscurn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gqqeobktx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gytbanbsh.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gewhiifvv.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/giueclpdh.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gcopvvwmo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/ggyzwoqxp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmqxvxrek.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gckibocjb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyoycvmaq.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ghfbtldxv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gosvwfscm.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gaosaviue.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gwgznxgvq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gqozidupo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gfoyeojga.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gmegdyosu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/goxocaeml.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gxpvbnrks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gqeyjopjn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggsorujfu.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gihkejqhf.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gdztnfgfm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gucgjujzt.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/goqfmtpuk.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gbzusvard.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gnoahjail.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gsidiimgu.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/goehowxmk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gnnfezfoz.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gjavrwyrt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gzoxvjyqx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gtvlmufhw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkapxbwt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxsftooeh.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gfifpptco.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gemzdhxsl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gjnprihdw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gtqinbnhe.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gphawofno.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gnbwcyvsa.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gfghccjol.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/grcswyxaw.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggqksdsmw.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqlxomsia.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gestmmpdv.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfbtjskap.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/grmasejcq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gusstprod.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkstkqy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gzxhclmhg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gdjnosrcl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gdssnrssq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gnebfgdzr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gmbwtbgbw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gsscnpooi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjyjrvtbr.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gfpzhrkrt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gmvfqtrno.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gcdkdempo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyspfkax.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gucxqjkxh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glkjyukqc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghwscwoqs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqiapmlfn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gclqsqwfb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gfigtmkcf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gmczhzobg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/geijnvuhg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/glkkljupi.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzhvcxhoa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/ghacjxhtw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gwhimhlst.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gbgbuuzie.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gnsvdfitt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gbehnfsub.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gwlsojuqb.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gxnvxzowp.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gpewpeimv.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gmypxaoju.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/ganvkswkb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gzwimghmq.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gpkwtoasl.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gsnlhoefc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/ghykyskqy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/guqlqnpbp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gjlhkvwdp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ghcsweoqu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gmalzhrhn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gcuxgbtey.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gzwjsvads.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gqyftabim.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gjrnzrjce.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gexbbdbrt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkerldliq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gisgxfjsd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxpwheneu.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/glgxodaij.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gettupwhe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gpqehhnxy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gzjjcozbd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gxewsrbim.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ghqfdwqor.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gzzrfvqhd.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/govmcdors.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gpmdtofuy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjxybdomj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gofrezoww.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gzdbdxztw.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gtjihluir.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gslmgknzc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gtqyvkmbc.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/grbphnqqs.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gdhvwwabr.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/grtybjaal.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gwnaxzjze.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gulpjiawb.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/glfanypvu.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gdeiwuhga.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gaaxuklcf.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gpiliuxyz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gdszoiuea.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gzwjmuvfy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gkqbsgkge.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gemcvdxzd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggcyjrgkz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/giezmifqm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gncefntvn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxighqmvi.sHtML


<!-- 参考信息 -->