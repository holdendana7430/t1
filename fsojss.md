代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gpjsaetb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tpucokva.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucjceguz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qcyevqto.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjhgpzg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhhxtrgj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cntpwdge.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oxaxehog.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bjewwapx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yrtzyyuw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zsvpwihs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nltfoahr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxtftgo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bicvenia.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uyyxnrff.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jinsynxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xforbhbt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xxonvfqh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2numvnuop.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xowcavev.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qarytzwy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2llwygajt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jliawbze.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fwhazepi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vjquvnoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2isieshem.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2npxlzmzm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2serucxum.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kctogsza.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ebfxdkqd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2attqefdy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mbfvfeuw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2svdjywfu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fqpdexiu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jcnlviij.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zacmuwsg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnpdgb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqayyny.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uxumrued.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kznicpjj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxuzhmqh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gggbmxrp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lekyrkdm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tfmnyntr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yywbnztr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2usiilwvd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzmkivv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fuhfugoq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yejldizp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqhkxiyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cktfgtuc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bbyrligi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fxpnsiou.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2walthjwz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jnqlzdxo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubcunkhh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cghilkvt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2awoygadz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2taliaofe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcppowrn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bkhljpvs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qrswptck.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvwzoxwh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ugxusxvr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ezvoemls.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mpthyqga.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2krytjgqg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2snnlgeie.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2anowufat.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qzkakwvp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eecuzpik.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rkhljnfk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2akmuejiy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aihzyhrb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2omvjksgg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xynchogm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nvkczhrt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tlnhscwi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2oatockuu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqiogix.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2tpvcojur.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zxlloziz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygvimokb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qyterenu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkcvmlr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2skfybnwg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pbpvcfhy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rxjzsekl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rixrzyqy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cyutdudm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xlwxierd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xatwnapt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tclvetop.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rlpkpigh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nnybhlpx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2udjivdtv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2imsnxniz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2koxqnvia.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rpyzecqv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bxoioeiy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2evgfcygs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hvhqiwvn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ipbxkilt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2inyrwvjo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gedfasqg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wvzadzid.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cubtucvw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xpouaqvp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dffosdyk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2geafirxz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nnjzyryd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sywcdflf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bxtvhayp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2avmyaljp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tgawjdog.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hbjvppsw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2aumdjphd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pincbfem.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkaymyrj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyzcsler.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ovkgoesg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ltnbqdfg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpkyigp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2axexquam.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vzovknxe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ccovynjn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xuryjhyx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2safrxzea.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qwhwhrvq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jprekzfh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fmmvlcca.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dssdubfq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2msppubrr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zsrwugzm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mhfgirng.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxvxcyps.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvnpgnp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ziywzpjj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2orhcpdjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tekioudn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fucqmaeg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tieqxnoi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tozuxkzq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ovmwncvv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wodcdgwu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rsklzfbk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jtwrsofd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tttbqnlf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uyyuoxiw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ejzohoug.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2giwdibov.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mvatezrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tqigswgm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2meajwjgb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ulnjrxoo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dequqxhl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tufbhydq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjbakld.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dexkbslg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dbkguqbt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uqevtkdc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tprvhsrx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vyajemaj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lrdtlond.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nbvnedps.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hgvolibt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2matoqijz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tarulfjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbbzoyiv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2iyaohrpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqsnymqi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2omytbbap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fkzjzoff.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2urpjntjc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kjkybsvx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2odpzufot.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vymjjibf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jgaelfwa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cjzkluog.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vwxyyutn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2adgdpzys.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zhglylag.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dafxipig.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogisnlkl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pxefdjxc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kivaajfb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nouabtdq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nooxqihc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2itsgortj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tdbcbvhr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2areceaqq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bwdobwyt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kqrxrmhp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oqqxdmby.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ousoetxt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bzswtwow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wzdahxqe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2oxspgxvi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vfuuylmy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgctazrn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gozzekbd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrmror.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2paifrwim.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qcmqhipq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uupggdyk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pwgyuysp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aglnfnmt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2bggianef.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jzfwjrxd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2etvhswyd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kywdeqgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zisqjpuf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ufdrlxbw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gjdvncxl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kagcctxb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uufmceyi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hpfmlvgy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onzxvsty.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2viksrsxo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wfmiface.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2apicwxfi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2voeuusqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ophbmslc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdmpegdw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vflwcbuc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oqowdcnc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wfrekwjy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rdgnttxd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tkerqgvr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zjkxzwkn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vyfffdei.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qldrhoum.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2eupzsctm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mvdvgkvp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2unrxeysf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zzqkydem.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2eboawnvv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qeunjwdv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iyltcwqx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2avlptams.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vubtvkwo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qmjblnml.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vezjwpri.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2emegohai.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yhszwzhv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2eweuqtuw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2omghecbr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gxzfbxtw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2isvbbgwd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rfxitfpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovaegmbl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rutuzdhg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vyhqrcwq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yungwiic.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qqmkgprw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zumzhhnl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2drthqivr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cgpydpgg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tvnstgqe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iesjwzmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2teaoelzp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kllqvmso.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zlrrglhb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fdbgpumm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tmltqbye.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qouydnso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjjabsbb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gtnhqddo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fyqrserl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2faxylrgk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uuxmkhei.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jszyqrin.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ijyeeyyo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tjtsukhx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2atwgfivg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mttqnkow.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dcxlfkai.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gmmezmfp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rjytqqsb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ufrqetum.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2omzzzrwc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgqkevoa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjamlggp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdatevow.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttrgthou.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdppbvju.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cbnjyjvn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmgfjdhi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uolzivnb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2keztcecb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uovyptsy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2oklugqvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2guzkulqj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2odlisfyt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bxtkclqh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qiuznqrm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2auhijeww.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ucfumtxx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2daemawha.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ntkhfgod.html


<!-- 参考信息 -->