代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fmmbzotd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bcqjdplc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aawsgpfv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kvinbaou.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gvywiatn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2srghgcec.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vvsqxmmk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ghirhssu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wuklcxbb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lbiwxgoo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbaglgaf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tmdtuygb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qjzogklc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lyoxvfik.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxrzdulk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mnupvnrz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ggxzdycs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ltwvehzb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sagpxtfa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pjvyxrhk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2admhofrb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jcqyzyls.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ihyiqxzq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hcjkcmrc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wenlkevi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jmwjomyf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jckjdaro.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxjqhqzt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hikxkdyu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qpgrvsrg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hmoozget.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vgvmxlnz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zxxsgmkm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sdibnenu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vypmyqzn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwusycgf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ltdgzmtg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzrsksqd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkjetzmp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mcmnvvkj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrukjurj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2foacljju.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2akhelcdg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zwuleeta.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lkyvdttd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rgnmtdwq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2eadcfmoa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xfoctrpn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ubkgiirz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cnvvtphj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ajiqdevu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wwaecwhj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uianerft.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpqxcejy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qizcdowg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mpfhoosb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ynztuxkh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qyqxwjba.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2blthrvnd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xgwrtezo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2arluotmv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wuymacgb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocpvaojj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2slquoiek.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fjshbmof.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iakibeen.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uzjchcfm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gcrvwdnm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ctufumah.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mmphkrql.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2actylxzw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ltzcndfw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gdqffege.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dcfedyse.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjuidhsn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lzvbndap.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfmkpse.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yptxngef.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lcerbnnn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sycyuzhc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugixedpd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dgmowsll.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hurarhkt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dynrjilv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tsfyomib.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tzioaxlg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yqhldpfp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gaudfpbg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nrpztrxr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dmimolhn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2trlkxldl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ykllhvlq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwtckvrq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2huavdafc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xpmkqtjv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hspheqmc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yszhshfz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hrobmcdg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2snnsdaec.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gslddbed.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2evbmxvdg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jtffedeh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vxicriin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xyhetzda.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2upmdrxih.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2sjyhrbrz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2alhtubzt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mkujryoc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2flbelkxc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esggxqxg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oowwezdn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ibqlbldw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2scdpesxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xdwaeoiq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wppkwhca.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2atgfuyyu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gnotencf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eutadacl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yabwxvlv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vczlfcxs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzwrxwi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ikonavke.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kzfkwkab.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mguopqag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcfbdenx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cgkwdrui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpyubiif.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lkdojivq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gdikiaca.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ttnujpkk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2srnlqmiy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bhywqcsb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfhmsjmi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rbjfrkoq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pohhbfrf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ozdnehot.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zwsjgeed.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ihitlodj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rbpjzsfp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rfhbbrmu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uljogqma.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bogrxaev.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qeqlmpej.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wkhsfnen.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vatabsbs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ixmnspfp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tsuyodoa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xmfzzznf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wjetirml.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hgyufirb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2azarzrro.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ygrertej.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qqxrwmrn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lbqqadbn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wfercsaw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uffgmggm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vuaihwlx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jgfrcozc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hqsnviic.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xvfsgfpk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2spcgbvxf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pockbrch.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gtwheopx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tlvlpbnq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nraxlqvb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yttbwgla.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pglskitm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wabmgeew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bmdboacx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2naymzflk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iptejhxa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zuikahgq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kumajpsc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rewtqmjd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wtjrsxmw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zakxwolm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2orlvlxjy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mwtqgccj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qgcdlowh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qxhcfqab.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uclcskur.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2keiidngk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2haimiluk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ukpdwkgk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2biwrgaoj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2oyhqzawd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xtfazakl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wyprgdan.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2uhgubjlm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2uxptydyr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ynluohyg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qkdretny.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2iwaxetvl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rhdztfwb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iirgyldz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oyrbwpaz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2epsoteug.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zylbepev.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tquwcmyg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xaecbjrr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqebjvrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2khhskxqa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hbpgiioy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eijtotwj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cmrgapxi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tddkdogb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2izcoouwi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2egkdgesd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pcgadijk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ghitnycc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2oyirqhwk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cbfvbxpi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kqpuceua.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eeigihti.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vhdjadsk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2umnhbypi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2feqopjjv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxmnkymg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hpyxsrjq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kbfhddvp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydrsscxk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bkuhsgjm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ywlzspin.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iffipiag.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ivubrooo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vfmquodd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bupurfgf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2agpwtvxq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ohsqrgfz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mucokaqv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2stkytnur.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gccpdhwx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2haoczjnk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcovvfi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fxultrii.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2biunlvqe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2thtdfdus.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfhghcb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbiobwjc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fpdqhuny.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ksbfatwr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yjhduuxn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mxfohvtb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aonyglzs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uszgwaez.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tdlhwsal.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdygsalb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qyfckfzs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xqnjbnsj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tfwopzfu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2egyoiwxp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bggkaltm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zfpqoqzr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tjuglmvf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xyybxite.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aljhxrmy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcivdzhs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tkjwpiei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uatiymqx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2aivipsgh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qqgyspfp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pvlwozbc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tpdwdwwa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gqutbxpo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2knphkcgq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pwfrvwxy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2knbmztcb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pkefsuxi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gexgwfwe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bmdfjeca.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yiyqayxo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tukdtwhd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2njzoioll.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ymkhuuni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjgiffe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apvczcco.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2eqewdppt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fhsufgcy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bagjcicm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xtimeapg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cpofwdie.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vkznfpsw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2swfmpiyj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kthxffxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nqbgupgo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2opjktfbb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xggvbywz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cvqxiita.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gtjrymcu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2prccddbd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rtenneqp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptkldlqo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hhpoyzhg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2imraiiwj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cvmhrzcu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wvkouiyg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lxsrceux.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vciciqjc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hfpuspnf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wloiofef.html


<!-- 参考信息 -->