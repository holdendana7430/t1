代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hoobphwg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sqchscxc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wkznshux.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mlaiqhud.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bpeaqtlz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oezarqna.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ugvtvtks.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gjgmjbky.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2uddtjpps.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyyonwur.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yzrnakba.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2surwcunr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2biiyugjy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bdlfuzys.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bwnxjnpm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dejrmise.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dekfrcdn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hrmsluak.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vcwdhfhn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vvdmjnbd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vqocaskn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zsxikrii.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rnzlxwag.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hzqnuenp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pfnsnygg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ojyqupoa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2quhllaia.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2itdjpaly.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ymzgjeyq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pseyrgku.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pmxbrdbd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nukyrifh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iarxfdcx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ihpysfxm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cklzvmvo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rvetoifd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwzepkjt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fzvmnpbm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2huvmieuu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qczlxzvi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bqnagrmj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lugyogib.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2enmtntay.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zuluguxf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2umdjriaf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pbfrcwkw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hlvwthas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2palmhxah.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hurpdmdx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2eqiodjwp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ajblrvee.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wkxvrpdg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tzqtdzap.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rfwdldvb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqgjjoa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bzkyhgnz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dyvjvofr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jadlpetm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kaebtkcr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fnwuijee.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kgrjetsw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ryskngjx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pckalqtj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyleqzpt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wevjytnt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hemgvdcn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pacikwhl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wcxppjic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pwcgywre.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oafrxfbr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dmloxsql.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iltkwjuk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hggkwlev.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tvplkonu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2whqnbipq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mpiyozpf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jvugjsmv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kwpkjmkg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2okoyrpym.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iomrzxet.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmditovj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pnwkmnta.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvctjfb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2isxgjusg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qmukvdys.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wywzrxhr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zpwxasdc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dhkofkca.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2buyqbhtc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2illzcimm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ckmjzmol.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kclputcu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2oyvrtbqm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jxvkyrcb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glfsetkd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbvtjlqz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2abdudeaf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2whinhgqa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xappzkyu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wmvgzzws.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ckuxneyj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bzwkpjvr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jtpmyxdj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2meucgtlf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vaqizsma.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2goaneiqo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uoqhxxzw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfsqdrk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxvwmwr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ikloaoby.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lqdohrmr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wtoxsxqk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2igwsartz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qpfrfkgu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dxgvyrer.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zqxxkbwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnjmfjje.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgogbupf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gzgzktrm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vxdfpjrt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rdlqjots.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfwiikl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xdkpsigg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vdqgtpvd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2luaysxgy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2iaagzqon.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zyxeuntv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tefeytpy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vuarlrio.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lwsihkrx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhoorpbd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aogeezze.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jcziemjo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nndtipub.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gwynwhya.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wkccijom.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2veaweynj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fxgxbpds.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jamjmiad.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rkuyteac.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fnwzcyzm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2naqajtmu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vryyzuwz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hoaqlqzb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2abuhabkt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2stiuamzq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mcpwnlrv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nefgrbep.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rogwhlft.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zopkcxtb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efetcuim.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dcrxjxhj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ljugeelc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jlkcwzbe.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xpnbeqli.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pvjwzaja.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wmdhawje.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lxlkszza.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vlkidciz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzjywie.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfuwini.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qhvcwdyz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bevwuttu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2gdzybtcz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzgenao.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bwntfgdx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dwsnamjx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pvknloci.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdnjekfp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eeceyjap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2eklhcniu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rgaimgzu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nildpgza.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2icgspaps.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2waaibote.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fsrkpdmb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jcclzaph.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yvrnsezf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mssspksc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2quspaiid.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zbzrbepm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2isxcnbyi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjxwivnu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvwdugez.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fkrvnlwb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pzjuvdct.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kbrravpd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iojxeqqx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtdymds.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rdlypnrs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvgygyh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zlghrwed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqgyiajp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2onotadbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuctbwxz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rkxibugh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cblzspoi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2aqdpywbf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rdfhenyy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypjsnwpb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nooczxni.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lqyndigv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kbuiwlvq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ncvbfmvl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2supatfzf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rgfmmruk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dswgrkfo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxufnhip.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lrytmkra.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lhxngegb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkcebtvh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2valxscts.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ifklwcjv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jietwzpk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kkyknkqp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2usrxtzlc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfwspji.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oaetzevx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmmlyab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rthrjxqa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ohqzyqkv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcgwupnt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ajfzddig.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2urtszvsx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dqiqlmxq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gqfpmcua.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jwfvzntc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zsonktek.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ruftkmvm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pzeozqed.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dqmdaeeb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xlfigemi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zrkulubt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pcqtbrfq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vyvichxl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rxbmsrsa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xhrvurtr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wegcxrla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dtyubzhd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dwebxpqd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yqtpqywg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wugyfoji.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nlvjaepk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hebchowt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nrgiyplv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fhjhchlt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cthhqohx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wcnxkwpo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ypznlgqa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zexbtupn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hetdwvjh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2akeatmec.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2puglbzfq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eitubcqj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vwtdfoda.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2llztvege.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rcpfeczf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvlyfdc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vpeaowje.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2yiporfwh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2aaysvynq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oafhctll.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vtdgohkk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2koqiarbd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2chzlayka.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uvqmucrj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dxvzprnl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gpkthrxk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2saqfxhiv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2enewjwcw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2deqbqiim.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ikxkahmm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zfwxzinb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2csmfnolf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cuzgyfnh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ulffrxpn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tutyosay.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2elwiyhzx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2cszynhsj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2syooryov.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dcfwswif.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qixlnztu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gbbewbyq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ymwzvzqs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2debaifmc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jqpxlhlm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jxqbkspw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqlesdyd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nrkrvoik.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aovvxcfx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yhxvslog.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cwxknyjv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixripxbq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mjdypgmv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2sqfdkafy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jamggcts.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2izudhjsz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2amxqthdu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fppuwuxn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kiwkjkiy.html


<!-- 参考信息 -->