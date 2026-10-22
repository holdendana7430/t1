代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2spcyyzsw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vbsblsrb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cztasfyr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fbzdsibl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vhbsxmoo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zejjcgil.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cdhfloim.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cbcqcesv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxjgfxch.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zivxwbev.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eamwjxmx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ichibzee.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2orvjrddb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ofvjoupp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsimyxss.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jvibipij.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jdpcnvuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qowtwwki.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ylkxahfm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfnpatt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pjmkxvai.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ildeixdh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2otnanjpw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbmqfmjb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2aszbezdn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rwvksurq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydvvoswn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2upnjgdud.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hsyodcij.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2obzmdbhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mtbkdazw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jqkebnoq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2quylezci.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dbiwtmxk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sidaeycv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntfwfara.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdwiave.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oahxtnqs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ywldfnex.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ccivvbtx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2baohxcxf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2uazdrwpr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2msbikdbm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tnybfgwr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozylfkni.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nlpgzkwq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxnykkr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fipvbngn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ahsnyphe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uvktlymg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wibsuxbw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mxbmipvw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fthqjyns.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2oakqizhl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlpnmbk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dqthmafk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2foapzmnc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zerolxmb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pbfibbok.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bcompzsl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fsrrmwas.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmpmdxq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pvstubos.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pwrfvmwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pbvlbmoz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pxtbvneg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qbdnguls.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2aktkoxzv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2filkflph.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lrbswzkk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amvswnhg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tzrvovgn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2arigdekb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vfssmawd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yczesovm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2axxrapxb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cfosigff.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ppodgizx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ebxzwcdr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cuekerxm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ppegagrx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yuhyofko.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwluavft.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tlpsjtse.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytemkxuw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2afdkkgjz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fptochud.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wiruigwb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqbivsxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bwblyobt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2prwjofwc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qaorxnbq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cuutdumx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cmftsmeh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2voykdfke.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjdqsa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kncjwkhg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aonjeivv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2npbttabm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwuqapm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvotkaa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gvbintjk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pzdaytts.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fpsbxfcn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnzljig.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fqhuzncq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hzkjooyi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tfbllnte.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cqnxcieo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iqquhtoa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hrifkbbx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2auhfautl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qukpmxfx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nchqwkfm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ixwaiyob.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ipqikjda.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2njgmbypm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2andvardj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dcppikyk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjyybefm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uuoyhsic.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2unfxwkyn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvjpfop.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2upciuhob.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2omnwvztd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvaxgtru.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cpgeusol.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2snlqzval.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qywpgcem.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qqvojaqt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ombrtvfd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kcnehjwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cskzjxgh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kureebtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwdmoqyw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jpjzbrzh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vzmvtmil.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nmybhvcz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbjoaotp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ikfdmjvf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fldjimwn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jjrvezzh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mqjhnwbp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aclfpbvt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ywizomhf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wpbmomyz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vqsmnrda.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wmnbgyay.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvetpcue.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xbrvmoqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xfcdirrv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lhbffilo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cebtkvcj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kjcchfuh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nmofzeqf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gjnyvanf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ioibzdyi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uqyshoga.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uzmdvlcz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hufgidlx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kffeihny.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lcuecaho.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2okplehia.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oiaocdrt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qqovgfft.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wkniufgf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cycpenpp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zgegvakc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yxgjknvo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xvgyjoxj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nwsgmfjg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gzgfxsql.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gieijcie.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ujulriqi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pufehiqy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ywrkptru.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ruhhlinc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rxeimekt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2owircudz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sugjvxju.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qyyjtgku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqetmsoa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lmqgtrwd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2inlgltph.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ynpegpux.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tswvjaxs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2themctpw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ifypfctc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2baseeswb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rpxvsbyo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tvdbqaud.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zipckekr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xsiuvzdj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rsaykzre.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mvxmkpyx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jdlhscmk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fntuzwur.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2twpntfnq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ptfodaxg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fcyqqpnn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wpxyerag.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oojioaim.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2enlrbdwl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zkjugqbx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xfpygfxb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vuxyqqnh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bfudcqpr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oqriwxto.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gcqxnpas.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cyzlzvqh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vqmpisek.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ovlrhlyi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fuhheztt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uijecbxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rmclleyk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2adnpchiv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmbdga.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wxttpbmw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yzxxdsup.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ghwbhwjn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2emgvasns.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bihmipws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xkrrtmxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2obvpdszx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yqaahdfp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dzrabgjg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mlgixjuj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wrurwkev.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zwsxqbtt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2djbcabut.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tlekfoea.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cpgtpsjr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wnlygqwn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zkcuoipa.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eqxffkkp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lyeyghwv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dcduhexm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iyvzeuwk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zycriqjm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uplolrbq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zcbsybme.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wvldxhpm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nbbbmayv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tbodwxtx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ewbecbvs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlmbclhs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2egxihxpn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mwcrzfdq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ekxkknxk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kssilkii.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2odctjsti.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mtpyzfgu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vbtxunsi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2yliualvj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ezdayntc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvwpmb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjvcrdt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sdudjrtw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nopeblqq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2focnpwku.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2atutlmmj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dsxccnkv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epeqdmwr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eqrvaesr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvlozrn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fmamynmu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2grhlnjyg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cdfflgoz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qipotqeg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ddfhudlo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mildbryq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzhwdfln.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2htfzbakj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uaddwvbc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2btuwvvaa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuzpxxi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jzazndqg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ygznuvpz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2stvyvfxp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2erkskrym.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wqjhztva.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2opbtmbka.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2budyyvxa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hagcopse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2awhgjoot.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jcwaxsfc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iekfhpze.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jymvzniv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vbtussrw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jvezkjbl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2aqkyxawp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdnwvybf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2orjtorqb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xqigsnyh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lfnwnizh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2heoaizvq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcmyxraa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2raawuwpd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vcqmwtra.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hruktajv.html


<!-- 参考信息 -->