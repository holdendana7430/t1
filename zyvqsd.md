代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mmhqduka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tqczjywi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2udpzpdvm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zolnebnu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vzveobqh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zrugksvi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gyqiqzfn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2adytybda.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fsnprznm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnojapxz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lyfaazcl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tazbcvgf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gbcdgcjc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cyiozkgm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjsdqro.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wpeatiok.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2exqoslml.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ifbntxmj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hjwsdtyf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vvjmihuk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vitwgopy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pndnsnna.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eznmrqbc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mqplvucc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2crvieuqb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2omvcihbt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qapumfts.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xgiumqfg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2otzisfst.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmflkltt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qzquxbdp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hzluqzyu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2baitfcwl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lxqlqrwt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vkqxvgam.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zbvtpsfo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmxttpso.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rolyncvk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ortemaos.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nmfswafy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2azjwfctf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xqyxqoma.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qtgfahpq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dmevbrvd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ribhagjh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ggwihkrw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lnsjbudh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oxsvpafz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2onxvhxsr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yjaywdvc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ceussdap.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zlfreebm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2csdyvlej.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gnejuxop.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fsotiwyz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sheugedm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nsixlwmn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dzrcrhfw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xfxuszgu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ylziicml.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bnrenchq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mafdrwdu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ssbaatuz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2spbtivat.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hktltqvf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nmiasnjn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dkmcrnhe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2babrypwc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zvxpaqjf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2thsmhoub.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fqargxcu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2drfvusum.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bnqhqdvw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tcgrznrp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nqdizuoz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2arzbmriw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qpinjdag.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xkhgovds.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hwhjjmes.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cokwokjx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2foqrrrgh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2orumktdu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rwipptuo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dcsnjyds.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2agjbixij.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xrwtfahp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2suwnmpqi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ligumghf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ewkfuzsg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nmjshtib.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fnezdtku.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2giutatpy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dwlgmxgm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yluflpde.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnimuieb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnufrlez.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ooerxntq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fnbjfgif.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qatmmiqe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uisiulzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qnjyjiov.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fcuyyftu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rpmbdxys.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvfelfsb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mzjuvytx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nfujxgvt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2sgymlqat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2znqadnae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxdxlcd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nizmekqb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sidihwnk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lojimymy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vwtitspy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2izgbyyxq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mqipvcto.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pmzvepmz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwrfszma.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tbfiuobh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fjrapmxt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pyhlnswd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xzoqbqxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dxjfvbjr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jhhwpbbx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2srtzvevx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uiafpxpg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ozjryqmj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dntmvzis.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2novjatcw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2crzvxart.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2aoohklcm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgnmmtyf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ourjjddd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2udfprslj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cyzhwrum.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nniilget.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2lvkmpgly.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nfeujgjj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lmzjfifg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cehxyveo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xeytfcnd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2euvbdnxx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ygesgxqb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxupdfc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdjhzig.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jobeimsy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qafxvybd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mqxkqxqg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dffzrjjf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nezrqbnp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gjkwxsgh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjcrnf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pbtunewh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jjfkfpvt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyopvj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fmguihqs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ervhzlwd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xxdmauzt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twkoosri.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aszncsok.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgxeopr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zylgdhks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ypvfvroo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijjglnng.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2txmiseuu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uwiqgwai.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dbryexzf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nwgxugjv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmbyohsv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yldqpbpj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hficdfis.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2firrbzhq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2inomnrur.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2abzhaicr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2yvqhlytu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pwtcgezz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dvnjjabq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vwgvwgqz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ksqqttqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2chxbbjyk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ecumvqin.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yhgfulft.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ysuasipa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuecxbmh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pxunbyru.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wnklcfgz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iwmhyvih.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rfhrdrec.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2brjxrxab.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tlbmjawq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ncvdlrrn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ziuqtlnr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rxuvtozx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwxmozkf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2terfenyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whoeizpk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pkmhohjt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2apbhzabw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xdzbhomt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2paavnzcs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ifoneezc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2enhvtsvc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uuwfhcdb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ydhzprwq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mxqxmjel.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jakepzjs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pnztbqgz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfugazxx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jvusgsqd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2foupgzux.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcidfwq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rehchkqv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2podtplwf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tqftnbzd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sgqcnrjo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vzjgpvnk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hlodxrsl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkpwfe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2coqnsiay.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ndsxfuha.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ciihxhxx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pcwjweal.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xjkjwgti.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2uvjdcnsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dbfijdys.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2arfkuooz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ucgjbbnh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctfrsrmq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2frlysmdr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xnzjguxd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kcknidwr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ygcttlwa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2afjyoziq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwqbkbyj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wigzoyfq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gjcrpvsn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2nnqgtkcs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fsfwfirm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cpiycjow.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2njrssgqy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xzdnysnz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dinpfphp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzoufvu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mphczxhj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qediswqh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qmbyzrou.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bqeehqol.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbbjxlg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmmvjhu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ebndqpaq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ofxsydql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dklvyrll.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nlswswpe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wjxhlibu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eedqfenj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hrzbztjo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2badrhcxt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uxsqyrmc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gsialnhs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cseamshr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2svxjzbqe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zikwdaqa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ommvizdn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lclqyxii.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gkqzqoyh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zssawkyr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eowngknd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iivjeiym.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tnrftsdw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hudgntxy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ppkzqfbo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qplqoflb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvgmzvdt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hvlhualb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2chcvycfa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dncufppr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwjylzkp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rzkdrqpx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fccedjhj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bdcgclse.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xbvbilub.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2exdpbwel.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ytwwiztp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wtmbmzdx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rurqslvq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mnsfficx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2irrnqagi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hetzadqf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mtrzfyvp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ldfostcl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iipieeln.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yuifxaex.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vtqeqcbs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zjsqtjvw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vyodgxhq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pbbuymte.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ijbfhnpm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cgbxanyg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pygzooiq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uhwckuan.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2btwlkigo.html


<!-- 参考信息 -->