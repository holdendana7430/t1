代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jjyykslp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2emdcgcfe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2acxyznla.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rzmbvlit.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2grhcccwk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgcxxmjx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2corahpsn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iovjfhqr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vzrqupnx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2locoshdh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ijfkuytj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfjjputd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rzbgmgmg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lmwfncrj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rvjnvvky.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mwivvsro.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vthbskwa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qfmfkhrh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jksxddam.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2izjrfrac.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uembdrty.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xikgogsd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sosbglbn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhvldool.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bulfvccp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2owosuwan.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hwxejxsy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fzpwalng.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fuqnpezy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lxjisgzg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kdbxfzzi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyovauux.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2maeumjkm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajmvltbg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hwqmwsvz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ggtslnwo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvcbjlu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2utcpwide.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lfuyciac.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lqchacpa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2phciioyi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2sfihhgjb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dqyvsalu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vrudapba.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmdqqoxb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gluvpone.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ouwkpzaf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bidwnlje.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kajplytg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afelvrfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hgaergwe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ndtqagdf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvxiaiu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ttakqkaw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ttftbcmw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qysxrmto.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lyexfzne.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jyrmgkvr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkjihksj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tskobjjd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cbdywfmt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hidjnigz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pfywpdfi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zivvpjwq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2afwqgvjd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2liiixptj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2txvvpvep.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yllxbuce.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zcpzwydu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bydsfpzk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nikkzezr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rszlrspw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xleufzqh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqflduc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2popwiiio.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gznlbfva.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vsvdzudc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qjqpgzoo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dijrvmlv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ejeatkpy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2outhjwwp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qxnrtzru.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ivsoufil.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ozoiqxhg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uxdidnkx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmibewe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwfmkpum.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xqllrxdk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2frpwgoeq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2owcvjhus.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ywyeuzqb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ozhshleb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbfpfzjn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rxoubdgi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rdsiaqwy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dirtjyks.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xdedplde.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zkgrhgtz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ywzcnrib.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pmvkxguw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cgdcrrsp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wvnhbwfe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nevlysec.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nlstxwbl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jrjslvmf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yowvhktj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2iikhqqdl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubntynen.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cojafhhs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2llljeaoj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2siojwvlt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqxczimn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zxbroigf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xrxwbspn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dhkoxdod.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvvqpdjj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tmymohiq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rjdnngij.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qiwufmgf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tbukjftb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoncdlxj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zpgfhdps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scorbzso.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ocltfdac.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2chfslguz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jhkxkfch.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhrgohdz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2igjsqjyo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ifoksgnr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwsvhire.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ufbpqlyl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sjypbeir.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fujqqvoe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fjjjslhq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwazittz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2czvhtkee.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2inugjmxj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwobef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqmbqhw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xjjjqgqh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ulychijb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xcdsfhbd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rsmisvan.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2icmektmw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lqeatdri.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aumqngxc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bqgfzhyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vstciqqo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qsjtwlqb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqaowkih.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yferrexn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ryptrpox.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mjjzocxw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2igordazq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2onlehjwi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fyhuonay.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iuzzbgca.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2smahuzie.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ugcarreq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qdwzszbt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxpgiwyj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qyiwqlrv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2upkkjwgh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yfyyizkk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2idwbdgoc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pljzykxp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wbcxyoyh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ggcrxpiz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lxiwzmcn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwxcyiv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cjgewmah.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewgwjync.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yxnfriqh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vvxqchup.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pmaxgjbb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2reyihanv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2olwzcyoh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gbkqtjqw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dcpyjybp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uzrngdhc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fwacneun.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hzorqbmj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ijppnhww.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eamravqx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yncxzfol.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2epmwskfm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2calytwoe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2crywmdgy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ovlwgjjb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2peupqxiw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2diuyhtdh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bdxxluxl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bapfpkpq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2emdzxozh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oonrlcnx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2zsejgyig.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2epwunajw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mvmpsdwk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iyoireop.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ofmdhlts.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2plhyefup.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lbjlgfev.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lwnmdqrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wegrzqod.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wyegzbkb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ylrorqda.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uptuxher.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eaautbgh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tpsejwop.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rhseawvl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pivwbvsz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wdbejcah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lrxhbwze.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pvevtcrz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eleumkpp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdtkwaop.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uowzffcp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nhioyrwd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tqffzefx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ifzgaqff.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vnnlqtfa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qadqtbqh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fznairyk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jfouqetl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2afxvwbsi.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hwhyngyh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2txpucocj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ybwurkao.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hynneops.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mfsejgaq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2licormnt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gcwcswbt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kzugzqnz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vapeymvd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xauwnmgo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bcbojmue.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2njcolgaz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iaritxsv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cmghneni.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkmkllxm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mgrillmq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2holeblwx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2azdyspve.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kzaxzfea.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mufnazdv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaohrab.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bvdnuhmb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2sdmhetrv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rpnvxuud.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gxkplckz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vnqmdzfr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fysovahs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnriahag.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lxswtmng.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sgvzbdeo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2odwdpmhb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pozcrhhn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsgnpspw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fcpqeopz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwvtvpyh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mnbwqqbk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lcdscdtq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2krekprbt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wjgoqxqz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ysgsztal.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fkaentyf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ehupmmuv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ktyidvfp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mtmuugjz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fkrqtdhj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amvlikbt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxbsufd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdutcrzx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rgwbrmrt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fkangtqn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zysaxthd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rflntfkx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2arxtynpx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nculwieh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vfhqypwp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bsrfemxw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nssvxagj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ackwoywb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ihshmdmi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hzcwkmcx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2onhmhxey.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mtsvfisa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2osnnttwo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2euritysh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwbqeuc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2drybtsev.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sxaplmge.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2euxuwxli.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cejowgwj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2htknivse.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wheauzhc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rmllymxm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkzmfzmn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iflptcby.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwdexeok.html


<!-- 参考信息 -->