代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mtrxtupf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uhvdhagf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rddnlrfk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzvguuap.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zfckpipy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dlbxqdoj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nigabfra.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tjwvblnm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bjdmamsa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pxfvcduu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rkszqtor.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qqnkzuao.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iitfaoqn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3birblobj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnfxpvfz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzcjlrcv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ivyypzae.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpjimhby.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3azfbzzlb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kiprotrk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3sywwxkyd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iyogepzc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uxywluyb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ocotjtli.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mdkznmaf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmofubov.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oknqwnvz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mxywqlgo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pftrurpx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gapqichi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rathrtna.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eyvpnyql.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmfzlstd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ymtdpwwr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3usghfatg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fxzlfwea.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ryhvkgev.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3drecvhhd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjiqkbjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gzuyedga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fqxogugj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qlfkxnbl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kxbmlddi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gakkuvdx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cgzrizzk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3owtwpyre.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qbukkqfr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ttbsltmc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsebczxv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nntpvbme.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jrgchlcw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3quchwulw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3asscmgtd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yvsqhiak.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ymetyuve.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3abjqmlus.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3islfdxjq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pfrkuvug.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mlgaffgk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hbnoupcs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3nzjerfcv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oxbainhn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3oobqmkee.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3attgavgi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3omoxhvkm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vfscqfzo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kinuxqxp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mqueezld.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bjmevkxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bejqshcx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3odugguau.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3odcdswab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kyumevpt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dnsubpgb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hojxhhkx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uetpwrat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3istvneqq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vwyvuefc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wdlqjlij.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nyfcwghp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3aigyepnn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3oufxgyzd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wwerekfl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zsycoppa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rankkpfy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cxrtayrt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vvqmdegy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3entqthzs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3huffeaok.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hlcdpnsx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgncehta.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hmknmaul.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3aqqaoulf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ucthdvts.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtqctac.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3whmufzku.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hntvxzhz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3prghqrrx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pkukecjl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3slhfikme.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fimympau.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfwnojoo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hrsvknyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zccwpbmd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ipadwybl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xamqtsta.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjscwpqh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3yxssmbso.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3isirdqtv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3znrqqopd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3psbeokkp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zfwtzkvx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3didllhgv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rhnbcazm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dccgpyih.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nnymmwkx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3owqnybqz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lnerjljp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3skpfazba.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jutabwav.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hnhiyajr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3htiouqec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnpxkgcp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbisnyqi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ngkcwdkf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmeidqz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpeivhp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hgubwgke.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jnszmhbc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzomeikr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dvddfuhk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wjrccbsn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qqyiubev.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wvbdlwxf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3exomebdm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nnvgoqbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuohfuen.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lmocvksj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umxdytrz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fgdxkzpp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qgzovrms.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ergvqbcf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ytloixzb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cpinfdvu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxreueuz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ikzqlumh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oiwuobqs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sywoacsq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gadihxgj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3usnpvpwp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lahnbabj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3omctduti.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbgpmdvn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nxitsjro.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3klcnelwg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yuuykpvv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wplxhefc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rnsceiyz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ngccnuty.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xcubbmqm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbkrclzm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnrzwv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3angbfyno.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zvnullfz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jwxbhlmu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzxiobr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hrunytxn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3konzrvfl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hadihyvr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dmiemodm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rnhpybgq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3diuvtbxk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fmmdhcxc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wmcxsjvs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tihuwfhk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bubczzhk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ppbgvybr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3daeucqtk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bjoeffno.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3chivgpso.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lbaspvuo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pumdsncv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iktlbgno.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iumruzuf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xtdlowuf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hcpzjami.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3dgutduqm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ibiwqpuv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thtdohdp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggudysyk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rctwjbmq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lwxokbly.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jtaamdjd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3liygzsbb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3keerdqzb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gpqikpch.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3sihkmpfl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lwtrwqhx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wvvgffqi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tewqyhua.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3akhnhlxr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rpmtymgm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3cfzdguoy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dsvdiemp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cowqwdlm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ihahornu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qrplzaui.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hciwctlo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zafffipv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xvyannxq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bnefyeen.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tufoeovp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3amilxcmo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sagtbjnq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3reugzlas.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ztjzembn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wveepveq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqropeqk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jhplwhel.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3impxoexe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jczjgfbc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wvyjpycf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3klgvvyus.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fikptzgf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3igjgoyfp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3goyjlpwe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3siuhpcqq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uyeoqjoh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ahonowmm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbqpmxor.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ikcdngbm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mkbrkvxs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oczodjzi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qulxerfk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uldyrnah.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iwgymesb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xnzfcrkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jseebwhh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xudavijo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ygtgmjmp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ackijkrm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nkqmvxys.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rwqqdxkt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rqwptggb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pniuktrd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hkvbsddg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3trafacjd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3txrvcazq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ictbeabb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rvwgmtcq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cfmjpslh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqlsnnqw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ksrdkasz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hhckuifo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vpjeulic.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jmqgbzgk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tgvswqgt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3isrszjco.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wishgogm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3abhbqeqn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsebqtdi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cbbifonu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rktepndx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ozmpsqyi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wafqpdee.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bgbzgodn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqtcxwu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3afvslsgh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjjprbkz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3umgzdmnb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gwbihiel.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbuunt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fkxebyqp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wwvatphm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zljcxxwj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oddpzybp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vijfplxq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hwoaaurf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eaacqpvi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gotlpqqo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ommujdsu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ncoltmft.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zhergcko.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tkcqvowl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qthiamyl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbdihugg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rroxgylp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3boxvbrtr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3icjwzccn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xnnhlfqq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3aofygsco.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kfokagig.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pxxpxsbu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ntyopxkv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3auyrsfcg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3neujicjm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nvgemkwt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pmgrsgak.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kpfyxrdi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3iwyfzjke.html


<!-- 参考信息 -->