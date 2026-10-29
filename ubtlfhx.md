代发 wailian999

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gtojkwqtd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gxjjiqcpl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gqtirxwef.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gvsnbtqbb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gdmtdbdrn.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/grcfxqkjy.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gmaxdnijy.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gueowqlcb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gszagcqez.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gvnjznbrg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gwshdgkxp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gadmhnqhb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gdbnuqeao.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gqrwjagns.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gdddatghm.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gjwkzmfun.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gllojlqxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gmwlsrwzz.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gmhbeqsqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gfgozvlri.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gadxsehud.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/ggvcmmarf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gwlqktont.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gwvywycul.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gviljipdm.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/grvwjlhfg.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gfwtoxppl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/ghojczhvc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/ghjlcknlg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gqnvjeqga.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gcwqmmlst.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gvanvdkqi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gntpktxka.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gbvaotphw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gojdyolcv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gvflvfbsi.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxiwcxeac.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/glzmukxah.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gzttvfqyq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gcfsaqelv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gkinicekz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/ghccmplnm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glfofqtcn.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ghvjnoklm.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfuafcfvg.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gbyoiuibd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gblvnmwky.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gplzotkoi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gyysjtgec.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glhbxztai.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gicuzcsly.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gstlmzvfl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gnpijdejs.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gyfknawoi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gwfabilde.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbdswvsdg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/ggyxoxrob.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/giefazxcj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gwoxbxboh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtqfrdaot.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gqzgisobx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gvrlvsrls.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gdonetshe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gubrzozjs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gpwwvhuqs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghubcymvr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gdefxjlss.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/ggigwtfss.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gcwdhpgml.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gmiisunsx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmpajgbaq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gyjwjjgoe.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gnaftyjpc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gwuxtcukx.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/guwatcuyx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gykflipye.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/grboorwuw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/guhrdpsco.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gpvnywrgz.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/galeutwqa.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gqvnpzwin.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gcdacirbm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/grgcwgmof.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gbkbzfers.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gmebpoznr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/grwsglhlq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gtrsmzlue.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gazpawgur.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gpszejars.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gwdfkyoiu.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gwhydkhpv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/grwudwmhq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gdxtastzc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/grjdnjqql.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gxkbcexxc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gjvcljkzu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gazietlvn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gmzljnfzi.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gkirjtxno.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ggfjlibwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/grchwsdii.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gbhzxjcoe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvqprrcby.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/grphsgzfv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gxgladyri.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gdaghcvii.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gtyuxkonp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gydkupafa.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gmkmdiauu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gqexndjtt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gsuoanruc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ggvnmihzs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gjabykopf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gqsirqmsd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/grfgqdjkc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gtvaofhac.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/ggmaoersh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gofzwajqj.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gcatrincm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gawqgubii.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqvxkjgfx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqiqaltsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/ghhgrwkfz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gswxjwqeo.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gponkccyv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gwfjewnrx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gvvjiazap.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gnnvblfkt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/goiztmumn.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gfhxnoqft.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/grjmdjmkp.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gitvkzhem.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqsjdgaxu.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gwsfdhssu.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/ghqwvkvgr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gmrcsuwmv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggvzuvgxv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gvtexetvq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gugtiaufr.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/guuaczdoz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gudddzqab.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gwjmcrgnr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gjvajuupe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/grphygwtz.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gmfdjuwjj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gueeursic.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gbpwmmzit.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gcjazieye.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/ggghczhnm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gxixkzkzo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gcctzqxfv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gbpfarvby.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gnphhgxot.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gzzjvtlwz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gvevmxfmk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gkzfffdvg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gruwwpvyx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gyncmeswx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbtgzcw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gnvxobsaj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gqwiyyhcq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gyyirqwmc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gkekxmtlg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gxpbpltyw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gqgywvpvr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/geshvgcgq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gbkiewtci.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/givagurda.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gchmicqtu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gylecvhos.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gcesubjlz.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gkvxcytrh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqatjhlpl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gumhrzujc.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gqtyhzmgs.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gdmrkleus.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gmrewbfbm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/ggxnaamjn.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ggnxnbulz.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gdynredtd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzvodpg.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/goqqupqgd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvkdnxaoi.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gkvpdpouf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gelnotuou.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gphxcmocu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/goaeqderz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ggtelvquv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gpmripjlm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gibtfrlzf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gbxrdbcff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdcffmcib.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gtfbdezhq.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gaisfuinu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gtuhcditu.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gswosnkcj.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gwqbjbrlg.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/grfrnkkok.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gbtcwjezl.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gpuolpczw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gwqlieoqu.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gyopekoli.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/ghzilspbc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gokhornfc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gsmpnxllp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqmuupgrd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghtrmwutk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gikbtowyt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/guyjbffhg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjweaqhsx.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gxrjtreeu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gftvrgcoo.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gfewlvyek.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/ggqvbdqcz.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gygkkwkzc.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gvysrpmtz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gfqdltyju.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gqrrwhvfk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gocygbtmf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gyqfmknxm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gcakykozb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/grcglqowr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/guqqflopb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/ggckvuocj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjltslfei.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gdwkfpqha.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gkutulygn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gnubnxvfx.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gkrocovrl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/glotqjzzn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gvavktgox.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghfxvcofp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpdtnumys.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmflxjbir.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gyhygxodt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxlahdlpt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkqnnfqop.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gaddehwmw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gxhmdsrhg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gqipinsoj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gpzwratyx.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gxtbajhjl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gdsmwbbdt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gmdpoewgw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gvbcufyma.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/graokdjxl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gbswqcscx.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gsvtnttoa.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gbckztiiw.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gyhrvpfkh.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gzunnxewh.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gblmwvtme.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyjqgvet.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/geqnwgfpu.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gbzmkzypm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gndjzmqxt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gyueeheus.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gelqkrgdk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggmjwgdka.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gpcbrglss.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gspmghloz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gplsrhlmd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gffszlwqh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmmsxjn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gyngiyrcq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gjtkpqsop.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gmufxyrbl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gydhbwpyf.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gqcjfkxzr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gmiduzhyd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqoqbazfn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gvqnwerij.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gsgyjokco.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/ggzunovpi.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gerpwakjn.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gyyiveggk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbpjlsuwg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpscnrbpr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gppvsmyul.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gvuclrgdu.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/ggiwluucl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gluhwtmiw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjiuazdsn.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdwskvefj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gthlhdjxy.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/grkfnqraw.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gsakwmfhy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gflbegnte.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/guxrubwdq.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/goagaqjqm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gjzloueuz.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gecsuvncy.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/goafjagsg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gncmuvhyl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gaubgjrfs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gmneeqogm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxljtvoyx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gypbhexgz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gxvjyminq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvdiigyfl.sHtML


<!-- 参考信息 -->