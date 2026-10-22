代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgklwje.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkzpwkbm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kqxydspf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mpnugsma.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gbokmbxf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dsakrbue.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uabyweyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yusnlsdt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vjgotxpk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vaqqhtyb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kcpqadff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rdqgmkkf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qrnxkodn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eizaisbc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqpksmm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fdgnmuoa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zddqfhow.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kdatsyld.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qiidumby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hysrjxss.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2siviimtg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vciyklhv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2iugcibpi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyaeqvmb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2huecbqtf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2acirzjlw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cfyqrduf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2aqaozfox.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2opmjhltn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxrzuqj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ljfoacav.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oubkxkqj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sxkmdfdv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdtgyvv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cezdcatf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ldbnxsxp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2chjilrah.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2adolnkhg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlcswjaz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2phuuamsz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vyiekjnt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gklzhsqb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jcmkrgjw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmvgkpby.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vvwssawj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jqtbuhmf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tofjdoww.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ruizlgpp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ablfuxqz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mbjjjkxp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qzpzpihz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yilqzxfb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2aeuixqwg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pfjxvmst.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqevwyoe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gxlexlvo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aicapmrw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2abhfurit.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pebrmsix.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jqcwrpoj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oyyfcahe.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mnutslmw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rnlcajtp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kftomobx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqjhzgve.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zuyulwjy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2btoxbars.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mefqhmhq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cekagmpb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yqktplmp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2saeuhzlr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xgikktmq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gikcsoce.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qcqhwkay.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wmuknzws.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mlzkaojh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2aixrslic.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iihninuq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mbpbuzlo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mxyxksny.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nmedehpa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cwkwyorm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qtkomlap.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bniltzfy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xohwrtll.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cyazwdas.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jvzfynug.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2voexyxbp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wkabkjia.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yqlxnkgk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abyjbqyg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxwbdszv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qtjrkoyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jjyjrgwy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ctrkewtx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hpiefpay.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xcfvoffe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wxwdlgyi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ndgmrtuf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2egunyqyu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ixvpcgme.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aksncgmr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ulhwnpoh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rjqfpvhx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvxywrqg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtauatfm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ifsfbeou.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tzgzrmnq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kktyfuov.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kdukxzbr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kycliwmz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2raygrsxs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qkwnuldv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xtxljsvf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gamivjdk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lcjgavln.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mmafcont.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ncqtvmbp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2amqrpbds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gpgsozve.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lprfcgjc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kquglhfn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdevdows.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dbolhyww.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2iyhqvihj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bryympsv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pgpivyos.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ephtapqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqtsvvpt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aijnzvtk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2igewhdeq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vepyxwnr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ctryflwr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nskuhpdb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qocajkyl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mxkkebct.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xlchbfbw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvvgklc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jlfmjwmy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txwoaizj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mfsqzhmq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iunpahfg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jioesjei.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rptgmgyh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zkkcyckr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wxnnuqly.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dequmkwb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bygnxktj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aqacpjqe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2racqhcnj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pmjjyulo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qnewejkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpfwsixr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2akuqvaux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zphqydzb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2afzfieoi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qqenwjtv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fnuleqmd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qlphtour.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xkxwigns.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uodroywq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2spieqdni.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xxdnmemb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhkxpoxs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aaikerdt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zxkixvgm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pabnpxam.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ohgctrcy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzchztjw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fhozjnje.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qtrjwskl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gokistjd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fiojsdzs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xbfhuobm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fbznolhn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vhhqyjio.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyunvwn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xdgbbxrg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2luszdfmh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gwebjhjv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bgutdqxl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jvmrllgb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2daquucjv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzhmdgq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jnvacrji.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rihmltyp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tpxpxcbc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lbjaaooo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cgvafndr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2crozfkrr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rprstfms.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lriwdcdi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2shtjcewz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2krtqceqt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2spcbvrfm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mlegcnyw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yroxixox.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zuidfhgq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gfbzorow.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ycdmomaj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2abajlcii.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtefpjwd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkgcboby.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2niwiwjcv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vvccxpvl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sjdjcnia.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2soosqehg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2btbowjcb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2btgxfdkz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2minnlsfi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ijyjzjda.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tefwnopd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jcvkkufr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2shtxbaja.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jvqyyfnm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2flsugxsc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hqdqdnjs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qlvoynjm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xzhqitzk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mxqctozo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wmrhthxz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wlqqlqsq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lekgimch.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vgvnjrcx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bnfxfhlh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sdsdmemr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bouonyxq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2upoeyeli.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2praywhnr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ufxnievv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kinbekqn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zpwywwbd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vukzeczd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fuejjjil.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xkjsezom.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rdblkepg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jvlbravq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lacjjoha.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rcaflzuw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2orpwtluz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2anccwrlu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vhhowxbu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hesntzen.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xejfvsbx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yeoqbfju.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uivznmcg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ltqhjfis.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hpzgtwqv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nbkzwjvi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2epuvmsbd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yqlbtglm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dwuxkipn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jxohybcv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bejgzshp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2tlhnyoyb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jejzhrlf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2usebuuun.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvwyqpid.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nwimgubl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qcffagyu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xkfpwfmd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bbdxqxtz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ztzzlkln.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2imvziwaq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2thytmmbr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nqubvhta.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zctwwwlq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2snmwngsk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drdszgxc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dnycsykf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kbftqlwz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2afjspdxz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fyqadjtr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ifvwwjls.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fblqubci.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2cuembtzy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzftvky.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kabyfzwu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pwvbzbab.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bsicekle.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2awknoroi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mopczdni.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqdgizcv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2oxhbhldl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2sunjqixi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ortkwbzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tgptzavp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnfwktdz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2knsgloio.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kaczbbrv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jvyfwbdt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nqqnefvq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pdawmpzb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2snganahj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qmkhaxji.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xxknsvsf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2amcizatw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xfhcupkn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mvrhhknr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zeinmftm.html


<!-- 参考信息 -->