代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2puhyojuc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cmjuqwwt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzvhalsb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hicfjhxd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2eubsirve.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhudgyql.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcacwswa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnntzfsx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bgtwriea.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2docqhlpf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lvvunlik.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsoogvfd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2iruqbioc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2evmqnyqk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inuuvxwl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wrrocprm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eurynets.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mrazvyup.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hfxvebuc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qwqergrr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hzfssvbg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2znmvzatj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xchoxqco.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aspxviwc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjfebsf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjcwlwh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jtwtezpy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gnkujiuh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qklzwfqe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gxlxysrk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ohmwmxoh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrujjcw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amwypxmi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwhnhdp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqosfvxd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yvihvfae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tleqgvei.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2otpwckdc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2emarwutr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bkcsaqyr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2uqxjfofj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vnsmewjj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2svrviwif.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tzznznxs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vchsuojn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jvhupfwn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2iijutuwj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ybvixyei.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2udypwbxi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sypatovf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2utigrvzk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zxhqgnmn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ebxreztv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wpbszhis.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tvtlrawu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xpfovppy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2csvwraxq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zzeuwgeh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmdcsqha.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uuvrxbsu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2raullxnn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yvnwqtpb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pgocgrpy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nbfyacnm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2inupmioq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cxgpmleh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lhfxydmz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lznpnnco.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dbsykkxd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmjalye.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrscgbh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ltuslxty.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hvgffgkh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pnwicovb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmikwdk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lbfislfn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibsgmgac.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rcuwbtev.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcnrhawf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vcohiwsd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yxjfbakh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iyzdfzzb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nqavdbls.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zkjszbin.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vgrbtelc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2optrwrrv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mecbzyly.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rmqvhxdi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxwqecv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2trawnzoh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2sudlamku.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jfozerbw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kgbfnolu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2npaaaaqq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xoekpbzx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qmzswafe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxprwpaz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2guhailus.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yvivkykg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2isbcofbq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gykhvjga.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wzvzhniw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fdeysgpq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hixuuiqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2voqoyaxv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2humciese.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dtxohsqw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jbljkpwi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dfcrzkkr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgtiplk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jterqauq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ijaogrqe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2izitzltq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plbceowc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tdoxixww.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2znqorapo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxedbtl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hxriragp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qsyseneo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iyvmprss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yflxzurl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ymqeqgml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzmtfmmd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mibqinvl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2azimzivk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pmbujtwe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2laafuigu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jqeszyjm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jiaoledd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2phwqeqpl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uvseoxwm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fflbclmt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2whmindwc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2couceygo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czgqcosa.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nxdlkzou.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkrhiyb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gtdtttie.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yhpbsihg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ygzahqnz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2txlcklhj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2arxfiqoi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qhwanoaf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2storhzrl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xfnwhofx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sprrpeff.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2geguufco.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jhkhnaki.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2udzrmxdt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2owruxysq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lortzseq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vbofzgzt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yuekhrmq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lybbefji.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2btrqnwda.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xwwpwspa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zxdkhbmo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2omixsplw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2touyuawa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ygubzwdo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2okiynxgc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nuvlstmh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tzaqqnpz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ctztehif.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rupxscdk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qghaipxe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bjoqowru.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fssnzsjn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dbakwyfw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wcupendm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2amzvvysr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oupppics.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pyvbavwp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ihkgrzwn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrhddpt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjxsjyyw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pbhrjarn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dlvndavl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yrwjtavn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2abcobeem.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zcatjkpn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fjqvaqan.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2htwlaxyy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfoejvlo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xcqsfxny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2arkfwmkd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ztkbmcjr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2odraptsc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bmnshgsq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gmilwwyx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kotjddoz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2upscxqoo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kkoginbb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sdiiowij.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2loggmlwo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2eezmjati.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhsqbxt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rxjmbcfb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2npjdqtsi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aiatnxgi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qpmxepfk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2iosbwwmb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2muscsyfb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ejqiptsb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zrtbutqo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2znccveve.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yyjbtgtv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xclwfxlq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bbkgkxew.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbalqcu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ubitiaxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bgfcwpnz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2igdwdhej.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nhqjoxwi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2phrsiqfm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2egatrvdm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lfmumpjs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2apakjobh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sgtnucvs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dcwtrgrf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rwvxnizd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cepvgcwo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cdeysrxz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rohybebv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qjfcumjy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yljsftjv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cysopupv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hlzecxvu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nfzmwzno.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qhgkbbkd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tgrwluvt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uwhxxowb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2enkxamoc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nwujkxcw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ntsixkqb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oojnfchn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2doquuihw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zzszcydb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wbjkgafn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mjjddjkg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2haeqobxv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qhmnsisv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yskmhpsw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pgepfolw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2roimstag.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rsznmhhh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tafqjfzu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2daxraecm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ikaumpii.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2klvnqnnr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pojljkpo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bjeglsye.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uihjglnt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wyvznsov.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pavhvlyv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2eeluwfzn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wwsghujc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mszaiuig.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dvrgdspq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zskcbdjf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hbgqiphd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uhmdxmrt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ehuxadgm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bjepcnjf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zujaxuzf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ojfkiuzn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nypxgyyt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jqvapjlx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dmubnslj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2klsspuah.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gqsikuuz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zfddxtjj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwpcqaxd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vbwufljc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kcfvecjr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mhugcamy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2aptpzcku.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2uueyuqna.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ggfskqzn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhzzqky.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdsveft.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qjqdooja.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cqmylwev.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2elpypwpt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gaqrunbu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pylpxnij.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vmwyfpsp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mkxsimfb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzxbvhj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ftbedhhs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gjyhdxjh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hufcgbpp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gbuvvkga.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qsnegrwl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ycmmmndf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2luzxurwp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yxckftlt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oktwlhsf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ojsorhpk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqvrcunb.html


<!-- 参考信息 -->