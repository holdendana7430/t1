代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckezaicr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xlsrqpgj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ezoelceh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2doycdimx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2lxzonszy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uslbboiw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdcozln.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itfrtgyj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qizrkdkj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xybhugbl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjtszjfl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2naqejxhu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bjsumcxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufxwmzbj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2isxwfrmc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bggvhzvv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fiaggeqr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2herxfdax.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ewzjxwmv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2snmtyxhk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2whpzikje.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2refeetqx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqnhkst.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wxmyqkne.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eaicboar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cmwddlhj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lnwjoxyl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ozavprvm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dxubmmqd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tyqothvk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdzfbdjz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2afqgtnjz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdciogv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jrfblnmz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2abmnmhgx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dpkwvbel.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2eaxenhpf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wgtttyre.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mrynamjn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xcfdssod.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfhdlhzo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nprweqmd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hcefevuv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jbafhnnb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrsoftz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ypjlrgtb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2brsfdkno.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lqjwhmmd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2blsichmz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cltaaelk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rhwlngau.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2otquclwe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ypazyies.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uxccsfhx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wdiqqsun.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2urctuqcv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cersszci.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drprzwag.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gctkgyfh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yestswpt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hzhslley.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ovirwbuc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2djsgrelc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2npaytblu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fxuuqckq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ryfycsiy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbugfenp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpajweek.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pedlkaop.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nklaiqht.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wjcqbnkj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2oiolfwkj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2iwpynnwn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vwwfvyhp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rwqadqap.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rbdzkuet.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2djdtgdcr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryyyxjmd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkhtsipd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bsighmgm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdytsjcr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjzmuan.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2duuqrdwc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iwspsszc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jimaalnj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lztnqdfd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uthazaab.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2esvifizs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ycpjynjr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vmsoijho.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sqasoooe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2krbuedpz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hkbciieb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdjypre.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dinqhltl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gomowqpp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rfbvkedj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uapsbbov.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pxlidfan.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2vfpcbiki.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyvjqtbn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hfbhitra.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sqiymewp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zmhkyasd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2npjcopim.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2heuhplxm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xsafyxth.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxrtavxd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2azrrjdsg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jljsijtn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bdhsvkll.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zlfvnltf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2aapjtntd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjuxyun.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yhxiurvj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulutthen.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zjhvydrf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flhizumc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxjleunq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxkrragl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qmifofct.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xxqxzrpb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oyabktig.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iiqfjdof.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oivpmspb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2doofswee.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jsauykfj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcaizrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orlsyqkk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ffoodkvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpovkflh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kfwshwpm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2slmrmlfl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbzxfvmh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2epmwwwmo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cvenyqfh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kcpmzmpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oaxakuvb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sxitvika.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wyklkwvb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iksowsns.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hxcrnqjg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dscsfpxz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jkrmuryu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2maxcdyef.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kkedljue.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgdrutr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eivxwyrq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lkangqvi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fkwajvfi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bvryaoio.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zilqvmqj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2smrytfax.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mmjdbhzn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2krpoblga.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ijbpdzyt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ecenznro.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2glpdlsrs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pjjsvouk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwrxdvn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kdeuoevd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mnokfmic.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vzwfdbwk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bnrddcjd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bfwbqngs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dqlbhaas.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hzctgbbt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2bzuxoheb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ngdicjlc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mmuavskw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eztpsmfx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hywcxedc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mppcjgxl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nsspyxxs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2oehojyej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2taftekak.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bvvvrtbp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhhznqb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2stokwgga.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rojybmxw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ueffnlcu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ywfvcvea.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xkhgoqys.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fqlwrwmh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vekfpiyg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2czpqugor.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xwghanki.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zemrdlhg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ituclspw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tugskvnd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ikaizdbs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htfnqski.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jctbwlpg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzarjll.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pjzkcwnc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oxwsooxe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2iizocrti.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fdrvqyjz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xnkdvxfu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvsnpvm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nslljqvq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vcoodngh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ovvyqcdx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qzwejgqc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tpepuuze.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wkrjnyuv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hgtjqccx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lyztunol.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sywuhxxz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhuufwrp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nhzuvsdj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ehbpixsf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dghwuttl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2psihdpoo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kzkkhlfk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pgvyyhyb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2proocmjk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2symjrmfc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2elwclihj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pmflsotc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uudpdhoa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rbsovlqs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nlixdhav.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2idjjvumw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhovwfg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vmeuccgc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqeymob.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2impqkapw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dvnegfyr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2caaitqgd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lmhykdod.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iihufnpm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kpsthwcg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2siyxygur.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ugyjlnwj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sycjgial.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mbaicmoc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2prdmhsao.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kdfwmtug.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2igojsygw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xyfsxmbf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdluaaqc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwxzfhrd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2flpysemz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2madabjkm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2torsfasv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2egodbejn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2alxspvex.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kygusqhw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ghaztimm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvibhopz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wugkgiqg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrbcddr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kdqwapwm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2afbmyoql.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uqnzdoxh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bkdhykyy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bbvtkgno.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbzmxtkf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbfwipsp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkfhugrs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uclxhbfx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uokenlxg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aaeoxzkk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxddprp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2iqfjlmfw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vxybiokm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfzvorpc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mglzypyy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mwojhiir.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cjgsjaxc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2esyhydyy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ijucmadu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gikuzxnc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2wwhrtlfu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fodwnpfu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hzxhulaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmnzlucl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xkkdunhs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxquwrp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lowbhwqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xkiqawjq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fpofjaeq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2equegxxm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2plqxvxbx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2phirktph.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ksystwxx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wqoaclnq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vgksfypg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dyihcqdh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wutvghvs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfhwzylk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvauyuvu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dhfbklnd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kkackymw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wnawqshy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mpzehxqb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zlvdbhjo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmauovmg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ezobuadm.html


<!-- 参考信息 -->