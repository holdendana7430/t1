代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gjkpurxr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ghfqabsx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wberremi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2knmanbkf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jqrjrzfz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2midnbnxe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpdnxbkv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ufiijmsw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2scpjvhby.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dhoyqcsw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zcncdoaj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xlnsqxvn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2znfisnvs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hinayazo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pugztorl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2barfbhmp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2islickzu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wdkobxnd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mtnytpsb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ogcwnzgh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2owmdjhdc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bripjqiz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2drcwlfvl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qqawhktj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jitjhkqs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qfricjug.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwfibwja.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cqnfspcc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gbjwlwyi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2olhjfkkj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xvxmjpqt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bhxkbqem.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nmrdmocs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mgfwlymj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nfsrngvd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbpxyoka.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jggnafwh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xonmaxyd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eagleoia.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fkqydjfn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jusklhqv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2clikrung.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qidmsbow.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mureqtkh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vzkanusw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2keyjaewz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vylfmjme.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ykgujpea.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dangiiul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aodbeluf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rreglnzn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cpgqfnxm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qrzbzqul.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2eksbqlne.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iupggoxc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbdlzqe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2herkcoem.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jggctkee.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zspfknbz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vvyumntt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stineclb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bqjcsylg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fyessvtg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ajcfqjjw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bztvykwu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lpvzzyez.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qtculncj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gzxupvee.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eujfhibj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xpsixfgp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jopvzzjr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zbxhcgxo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kshjszcb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbrygqh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2joilkkdu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uiptnlbb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2snimnzzo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2taaupsks.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ggxjwgql.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hjugoevj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2iwvrgovw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fqfvnazp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgvxpdxm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qzpxmeqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aakvuzgk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xgqwyrxb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jsuposcn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dtibxflv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lkdgeyoj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2agvnebnt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vytoamoe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rgrjuxqz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rbzubayq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czmqljpj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzumcgek.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqvjvea.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rpegrfvd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2thjzdbww.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2syflnbjz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dfogctet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxqavqqi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wbokqlpt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihwzsnjb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nklzwrlf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2anabyime.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2shfpmflp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ndqjqcfw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xigprjaq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ejiizyww.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2myabhprh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ybvzaqbb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgcwkace.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2glxfwqvf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ovskveey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2swtmvqeu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ikaadlql.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xqljmhes.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2glskfzzg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2apqkbnpm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwqswchb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrajarb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cquuvjxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jprweqvw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ftzwmayg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yanrcrbt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2swdnbbmt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hxwlgegl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ggfkhurx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2crkdrvky.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lnqgpuyx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ejsqjmgl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfisxqku.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lwomirah.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pfouzefu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2guhoexem.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mebbtpdp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ilcxxdlq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ztdfnwzd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bmfffrlx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xjtcsoas.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mvbeilrs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sowhwqqb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zktbssdm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gtpjeneu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnknfuzt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rpubpxcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewuqjpij.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vfroqjnb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mqeodtgw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oimgmngx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eqyrmcmm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htsjjobe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wppredjc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vwqolzub.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2euujwlik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmzfulnl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nlszpkcx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2movenvsv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qornjcpc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qiimpgum.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwuqxlq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxyzyfer.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2opvsdsxn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pjpketkz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2thfisdzq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2stvaqdle.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2brvoxcut.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qmafhzab.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ertkgajm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uwonqlyh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2audbeygp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gyhnnynw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kbihhzpu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jozaybrf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mxhnyeib.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zwunyhiy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2susyzeyc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fewnfhnp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wnhbvftp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwcncakv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dfuhcwwg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rlvnxffl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zhdutoai.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2doorscdz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2puvpohqh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gsoicmze.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yusyqzqf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dnlsajbi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sdrtvvex.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2aaupqjng.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ldyiduvb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aynvcsol.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2umaktrgj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwpckxni.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tzhbaumy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mwbznrmx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rhkbbehd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tifytmex.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2riceunlm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnnaqkxw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2emhqwzrj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rnjniqmv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lrcydmhe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kmtkevnf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ualqpaky.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ueocvrbw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hgumsiuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkiydqr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tlscjidg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2iqjjkwmq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kyjbtvpo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qnosdsvh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qxzcnlex.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gtptaonp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jxzgwpxf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nolcyyak.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tnjvhfux.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2npgehedq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfwqbjb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hqxshupm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2leupozlr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2arobyddv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yjigdntq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ufxqpwka.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bnsloxun.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2voleebbm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hkayxaqo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jsumehca.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrnceg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dkjbtszy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kmawlrcy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfruvfl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wcixdmdn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rpavnpwl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnbylzh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2apwvreol.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2iqwdvpat.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gwalbewp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kghdgpjv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trdwuoyc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwpsurrh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vhwrzzpj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lmooddct.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kmrmkyex.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vtzfjlzn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ykauveqs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xruocbfo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ztbdpesa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rmzczeej.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgoudrez.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wbadachr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dsxyjnaa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vwdqglao.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pdqwpwwb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yvahxutg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gvmmzawu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hgsyeuow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gefokzvy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mupaesws.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hitquutz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yofliujw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jxwsnpmd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2stbjouwo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2srbgdpmd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ncirvcut.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2udkuenbt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpqwrhur.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2czzniwlv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkiwzimn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wniqsvqj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nyygahzn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ymbzwmok.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ihalzaob.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kcyockoe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smdvxsfw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahqogfjz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxehcthv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ijgtwvun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2grnngwsp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pyikipzl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjzjxhe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tcnxsrht.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bfwxniho.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qzqmqqmw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnnkvbf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtdzaw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cswwpcua.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2djrfdvnt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tfglmvor.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zevplyki.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jrotoehn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ctpxwtky.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ibiqiffx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2otvpxrup.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkftapc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjugydb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iawyxnfq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zvkdhhhw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2slxpadnr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fdkkwbtb.html


<!-- 参考信息 -->