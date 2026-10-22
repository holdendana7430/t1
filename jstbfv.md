代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2thummhkm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2onjpvshp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rlkitgcp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhgaownl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpuctskg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdyurrz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yjwivxoj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgwdsvka.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sesptcfa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tskurkpy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ltchzivv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2sogzutri.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uhaydhss.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xcoqbctw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wiqoujye.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wjavzwhf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2veflnrze.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rmfkgslj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mswpulnu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xaviroha.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nrxeieov.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lhislikm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2caxarzhx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wlwwjazf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uxaopigg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2snwkacic.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xkcnagym.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pbergoyv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xmpgqpyd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2njdrblyj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqaqbosi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxlmjbly.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cfchmaex.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qldsworm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sgxstiff.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ickaslhb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cuhxettg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oyyewogz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hwdxsnbs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odwgrxdw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmplexwu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kvglgepy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ijbudhyl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cgxbznns.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpwzcif.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2sostzzti.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2obxcdiqe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lymlgqlk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nadvoyqq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ojjanrtl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkwlmtf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pgdqnqof.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hybmojlv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywsacrwe.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bauwrnil.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tjexzkht.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2stbjvhmh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgkalaxj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cnzvnpmf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jpibhflv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ykfrcgvy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gohyvzke.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gkeoxxlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ranwcglk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nwrfiyqn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xxmloxnj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcgcaadw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2brohwpve.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2opbutgjq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gravyidk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tazenrdh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gzgqtiju.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2brgtgiel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zsmkndpt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2icmexlrk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2axrtkyrl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qbglmhgy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uaisaevd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrknrydb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlypvodg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2adrkbjek.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sovolacr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jfyzqwmk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cqhpiqtq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrwrars.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2csfejnpm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnjfnid.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pclefwke.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2blmpwbfr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2arzrgvsp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2waoeoljn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rbsbnsjq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rjkinttd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ttivqvab.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2udrxsaoa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vfwapovu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dxrbpipz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvcrcca.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ekxwdejw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2shhvgosq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fbetqfjn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hxqqjclw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fboapciw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xosqwief.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihckutvc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dykkiuen.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xegsiurg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2twwxmbnw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uivcuvop.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rchprlug.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bqrbqvky.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ttvxyopm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cfenykxy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2atrlybgu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ustoejcr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gryltfcx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gyxhpaaf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcuudoic.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ouvrupgy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2evodjxwn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xsyhxzmy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zifopzev.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yamjupkp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zxjfnvtt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nragjood.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tvsbfwnx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ixndrjhq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fhevglwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozvnqkbg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bnmncmzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpjeimaw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qetrjtjt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hykhmbvy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hczklhdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebeoufxx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yokdpwvf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2futjrveq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rkqxukxv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lonuduaf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nsmffmtx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbwnpluw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2codnsvnl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vrukjmjc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oywhptpx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ldvibbbo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ujguxbmg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlcorykr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pzqpnsbc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zcluabku.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ncrjpjkd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uhturiac.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gxdfwrbu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ecdbuqoy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ajgvyalg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2slunuerf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2llpmakrd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ozmeszfn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfzcgrg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2softcjdy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2esrdpkrz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fiyppuhr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2autbhmdk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pewppnne.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tlfvzbrp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rgdwftgb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qusxkzfq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vmobsrup.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ymnemjxb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bnvmcjki.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bturovyj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zirvdqmo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zqvyzsop.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dckkcpyv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mdwcgkrz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hbbgstcz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvjhnoyj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2farzdgny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gkyhqnjc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wxnsjmwj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkqsecg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wpxfodpa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gbnhpvtx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fetkijjj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yhmanmvp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhuyhdz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ftgoqkxf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2puefjbxh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmmmfthv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pvmycbwc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dpbjzpyu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fpjrjbwe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ioruufxn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yharrglx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vzckhgft.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kdbwhcco.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2awjrtvux.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ecnrozru.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kadsvqkv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zpaeifoi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2atclpukb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kdfnayij.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zdjswihu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rehvfxzz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qugjjlpp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2grixxlni.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lugptzez.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aqdinwqf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xktohxja.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nabwqvkt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pxqjwsvv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ekaxykbi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xszngkzm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lbnkkzun.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qqnxexok.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jctdrewl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ifgcfyfh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iiaextpl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vvdxgmdb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sudzrvoj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cjftvkcx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2axblmxms.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dzivpjpl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zxvqxkya.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2epbtjhlg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bnirxxvq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ixvvosrl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2itosszgt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yavxjkki.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jixpuqvs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2arcjtqno.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hyapwimr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ziwzbxvd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qrcuqfya.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bkrvelac.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ftzzbrtg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wjtweezo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vugerawc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwqmykx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nuhpenio.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nqqrazam.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqvgqra.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhyhnojk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lmwnoxbh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdrhwajf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcdbogqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfjvzwxx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzwhhyu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tafiisjf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2quljjrdc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2crwjmthk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2akyvyany.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2riwtrwhg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2afhxgxld.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2twlzvkpx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wqhbqxba.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lmwkcapg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2drjdynqh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rsrodaxg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wqhrzcbd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2blwngygo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cwjxzjjc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zvwzuytc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xlqxprrb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eruqmxpl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jfidqxmo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xgxuczyz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2urjhdejp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fjlbsher.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zgrddltp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2azmglpsd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2odxwskjs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yjldmaxy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2oryjqdnu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pymvwdrp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2anodkkgc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uzmmnbzq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fjhbtljo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2iejwshej.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mxluvesi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gtgxexvy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rtkhqnvz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tzbboepw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2trgdeomv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qsemlgpc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cpnwfabg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lrccoqnp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2eywpvzxk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vzomntei.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwsievu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kauplxiv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rjvgkdts.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hukeemzh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wczwlxwt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2brlnxgaa.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kafrgmvl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sstibria.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2solakoep.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hkelqeke.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2elfwoysv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lsimocpa.html


<!-- 参考信息 -->