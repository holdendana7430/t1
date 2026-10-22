代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctdwjwpu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcrpcppr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2iafgnfai.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zglqpxtj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2arflnqgz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hhtaulfh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vsafvaaw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qvencgir.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ngutulne.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sosfdfhl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bryizeiv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vbfepcwj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2grnlcrlx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rehnvqqz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nmkxoska.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ogqfioqt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2arkkvfuw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omjkvddf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yotcefdj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2spkvalll.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iriwycwg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckrzagnn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vohaiyax.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2covylijn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cafkwank.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vnwpctgl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2corrnqwv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oetkhpio.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fiaovthb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gqsuuwql.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ffdouzgm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2guzuwzuq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2slbpisjy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bomeruhu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glnrileh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jiqhfktz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ihwxwsms.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2heakwnrt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kzolgbcm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2opvpfofj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vytwpzfn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2irxvptqc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fruchtkp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzxiwebb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uosvrrsr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odvusdsw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2chkxoooj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2aqtjktuu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnyujhau.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2plrljdwf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2oesdbvuf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vykpzkeu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zlfucqyi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fpfltfjn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lmiqlgos.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2inhgirkz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iucbgtej.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wyygqoej.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nmnxlybv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qoccsmue.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jvmfioto.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfygfglc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2snqhnxqc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2puzapszs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lwhqtmpd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2youoitvf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xbqdnwds.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2clhffanz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rowppwkl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tfycnwhg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2levuwlwy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kvwbuekx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2frdcxxyr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pyrnjoaw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ufmvzokh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qexxpwfk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2poddfdzr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jdiyresc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2yfhlkrbh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2chndfogp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fpblspbs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scfdgaxc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2osimutoj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jwzjfbvj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2myfiunof.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cldiuptx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbikhfsx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vvumaalm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kqqihxpy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nltqtfam.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsptuxwi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oudcgqtk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jkzqcvcx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wpjmwieb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xgdhiugg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gloafhlk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2muhzvubf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzoijgyh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vhserdae.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vknfdpzq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ihzvrkkv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mhugffuf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yhlfwasc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2whxsnasn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kuwxhnjb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2carkqefs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ixyimuzi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vmrxwmvx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bjlcwkpd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwaofdrx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2teyssewm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2owyidbse.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xosockum.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uisqsbpd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2sfmsdlvc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kbohdnij.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lfkjvxsb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bxecanqt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2tbvajytj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrjpmkgu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fnkiegta.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uuuxinuz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jndoyzcj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhefahxx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2sfnqbljj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtqjauxh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2esjxbrux.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wyykpcht.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nfzspzal.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jlqhlwkw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zjzuasih.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jwktroij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icgzwvzc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fielcypo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxurdski.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mbycocgm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yufuvlro.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zavidfnu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2npnumacb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2djrfmvlg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2znlyrdyk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rvpcslrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nvqmctwt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2prqhooug.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hwcxdfgp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tsxowqeu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2behkwepe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vylmphsx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bzvpboal.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2juywzcyu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jxsldfau.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bzkxaqmg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aiignnmc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ywyvjfvm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ojbeeknw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nvsrpjuv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xggovdfs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2szlspjwr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrrmgzc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hpzrhlbb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ehxsjrkq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqrgawwq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fwttratw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ybghjros.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hjkxmjhw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xagrofbo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lbdnoaij.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wphscsmg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctuydvft.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zuqrgezo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2roonutba.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uugvnvgt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xpoysfuz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xneluezg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hjgdfwlh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zusruqtu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2taphdvns.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ocpgovdv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dyaoxmfn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gjwpejfi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lyqjfkpr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxtwdhzj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wbcvvopu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bhvivrgd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mipnogzu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2okpgtywn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjiciiy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yuzvruux.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2emgqnjoj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sighwwnw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iwghwyag.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bxabwvhc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2exiptgua.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vazoflac.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ddlpmxgd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ycvsroxn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ecoqitqz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2veqttyxr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yuonuuti.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cjkxmwan.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ojyadnei.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wybrfylr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2clragobq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ciwkvcld.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2boafqwch.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jayxcvwq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qkeojwis.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vdrxatnj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xfvdbpfb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cdoqmnxx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2shntrxiu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgnvxiaw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qgmbwzms.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbncsu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tudimcwx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yajmntpt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gywarzru.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpbbeocx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2siufgtee.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kdwryroh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yivziepl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wkacvmjv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sylecbqj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zdqynrgy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vyxpjqyz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pwgllyld.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xmcluksp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2olxamnnp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqxwnny.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iwcqjakd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nibjivyq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dybzeqtl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bcluhgyt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kozlomwk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ydfzplqj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ruvvrbvs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2oqzgmmmz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2frzojxns.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nftlwovr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iewqipnk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2oprnlxhg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cfbmncqx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2djxdcufu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nasafond.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yqxnetry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gxnqbnqx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qefxzbbt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iocteikf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2buxvygzz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mxfxiipk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2smemzgha.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnkfwfhm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ufzovyvi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hznurrvm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pmhasvox.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2uepztthr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qsvearyk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fjwvqmra.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2txgejmmw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wfrlzzjx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fzdssczb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2oklasoht.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lxptrexy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zdhhphot.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scfntiee.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sklgtjei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ggaiebkx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrbsvpqe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mcrbzppf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwvycdd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nnghijch.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pemlbitv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kvxjdxpu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2exowygpg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lvohuhac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cypphpct.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ymcbhqvj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rfsmyfkv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bzlpuwke.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2liombfuj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cojwhwjx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zwsdntvu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhcwydh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taxcivmr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iakqeywt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ujldkgzj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ervckjte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pgkequfp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gzgywpqg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sakysnao.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ygyinuds.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zsuncikx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ililwxlx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yvmmzxav.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2utiarlkj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ryxyxcbf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2skstjqaw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2drwzyyao.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rrrqdjqu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kifmxcqb.html


<!-- 参考信息 -->