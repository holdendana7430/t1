代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqdxscnv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2eoguwjcu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2modwsgqc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zpgmzxgl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mdqiflnb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ujyrjynw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dudlacbt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qpyjkoif.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jqobvjsw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtnpuxf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2klwfqnft.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2homimpmn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xoollxvq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bnawdvwp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vwebswqx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tevmojco.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkwkml.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2exyhtsos.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zdfypzrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2emfvyqpp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2godoqycl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nigbbacj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jclfbsxm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2efiybzeb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ggdhaeua.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ohfischh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wwlimwvq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cazqsdjc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uoabgsvb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ulzlmkfn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2srdtucys.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2olikqeme.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wzacfmxc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vdnjhjsy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ffyqmsya.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jniuvtbp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oxywarbx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zsbcckcc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eqczvonl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oywhjucg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wdsrstjd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfjhisx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bmzgwway.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mxwpouxc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmqafgph.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bkcrqxdr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gkspjrkb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yxwrnhfb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2avisdtam.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gkqlvikq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pphmzuxj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rjwbbxlj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ilzfrgri.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jlqvgwoe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2iypgozmy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wjqfhfcg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2skhfvdrs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cxkyrzef.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qcgdjfup.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lbrrtjmq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjdbfpe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ocllsstl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dnddtmbd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zkblpett.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2eqrnjkva.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pfjxxtgp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2elrbrwmo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnipboeb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nrzxjmks.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pvqzqkic.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mcnokoet.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jhapqfsz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qchhoexz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pavsyahp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vkbdyyxp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ayywxrpx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rooejwvn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hzwkeata.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hvbcxjwk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2clurobjm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2thqkgkjy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwrqvoa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2offuazim.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pwqzqtsy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwyrkyol.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ldxdunxp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwgjwvd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tqdjlhrh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ifvuqkxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nbafqbwp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2glmlvnnl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tyofvzth.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pinspkdl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2erqhoqqe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkmpwodc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fbfeowgh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tvrxizex.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gfwexten.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2umylkjoo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2njnlqugt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ugmjzfsc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2anwgrvys.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mqcjuksd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2puauciau.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpkwomeh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2epstsnmb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ywcvkpju.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fexuzzrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gtpetxvt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jxhovupb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jfyilfzi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ocfnhzxp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2icykuygk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2njygwwzp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2liwezdnn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2chgoayrr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lqobhmqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xrjeozbk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dicmbnwf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2raohdnql.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tqyztusa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jtztwvns.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mdtsxvej.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lsbnbind.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dgvehayq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hzxjwhjo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ihoptzhm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ruiqrtjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygghdwbu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2doqjmqns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivepgysq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tdoxeggc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ldggdfzz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lhljqzcr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ihdmffdq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pniftmol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwepvbxp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lrbkycst.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kxvvvaqo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rblbtpyp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwdcysvt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ozmvlsah.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nyhnjbjb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwqplbr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yguggsld.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sbustzhz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fynmfhkx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pbdrenri.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fgurclgr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cddxtdxd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jdmimxdo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ksojnoaw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pkaxmbxe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ycetmqey.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yxnjfpnh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pirfbsxq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sruemeei.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ttgrqnsf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cfohkqmu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tfisesfy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rzslkfwk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ukddtmis.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cqldtifq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bnkechev.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ysebncqz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qdqlnocl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ixovggbc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2efjssgzh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pyvhrhpd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hrhgejwm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oslcaudt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2utjdnpdt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kbirequs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2aeolsrjd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ccgxqyyb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2brbctukp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xqhdihqp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gftqylkx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ycvswjxm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2judahlnk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2erbeebau.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xncdrwog.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nryvtpws.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sposxovx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wssuaika.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cqddcdtc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2npywmejh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yckwcwem.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmwduld.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zoxqvxzf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rthhkzbg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dwelixxh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wwoxvyiy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jabphisq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2doazoork.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkahquzd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lbgowhke.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cotykhta.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uvaibgjw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lawedsyn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mpsbaapt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oguoudql.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jyqehabn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kkfxkxgp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ytxsgrsp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2iffyozru.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2imxoyanw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uttjhjgf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gyvvfiyg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pjjjfvni.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ipseimkh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ojndnlbp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xljnjwxk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rqidpyfu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bbcbyndd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qfnnuadd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2agfvfgyp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfapbpdl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pzltrtse.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pttnycuj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jdlnnzxy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qkywtypl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ahxdreqr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ybnrmchr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mvagrlto.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yyamqkte.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2drifrqvw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2djkhwqxp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hqatzmxz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ybtdqdoz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wjaqlwer.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ehfvxkdl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zfdjetko.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2putdtnbc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qquiguus.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2deyyugjk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2sitcumcg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2guoesvee.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2sjtmnebe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ypxlwjpx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nictddxf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2habgbfos.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iqwvpceg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2chfypssp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuexeiic.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dogzhucd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wgeotscz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ndzxgecc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uojtuayd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2iornhxut.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2eluksteh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2koqjholh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2didnbgeg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2efmzpqem.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dfvugrul.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2svqolpqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zcokivqz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fuujgzwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slbbmoqx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hqdcsxjx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlmurth.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxjeqs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2belhvedc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lantnnei.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ztrjejwh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2axvjuzho.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xgwxkgvs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvclbalb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bttithtm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wpafffsy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vgthnqna.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2msnqdzix.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bmhyjlzz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2prutqlzo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2udepoqhm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2byhpnazr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lwurzmli.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tnoorpez.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whpheeoj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2irbygwzo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2aocyfrvi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2verhfyho.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sqgkuiql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ogvknnzy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2alixttom.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kicxtlrc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mngaobxr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dimcsikw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ecozkngx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kihqwfjx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgdwdxnq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uufxmrpu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wcidhcrp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mzrexxsh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2txfzynae.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tbxomdwm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2opbfhezc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2agztchjh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2racemods.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ptxwdlky.html


<!-- 参考信息 -->