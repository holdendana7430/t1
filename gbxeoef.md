代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gaujzcjmu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/grpgbbjhf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/goxthgmhk.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ghanhcfdr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/guskqdbfd.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gcelfrloz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gphulxayf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/garejalgk.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gumgpuvds.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/giivolehq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/grwhxpmze.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/geiaapksk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gscekffxz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gyojmefna.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gwgewdkcw.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gysfqsugs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gnjkwxamm.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gwfznmcbn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmzjvcqtw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqtwasfup.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gaseqdilv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ggtwsxkjp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gqwkeedty.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gjehztrtv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/guodzspgd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gspkayqir.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gdkyjmbfu.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gqysxqcfm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwszirn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gferrxxfp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gkqntayxf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gakldtvgf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gigjyjicb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gjadmyied.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gvqmjvaej.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/glckfgvag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gwogejsbd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpgjodb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gpoweyqlw.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gjrxtlkjn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gsayorvec.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gxlnfvcbn.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gifxmhdci.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gkzmadrpd.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gtrklwedb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gkqvadbeo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gwssfzhzg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gftneqjzj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gdaqrzuqf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/grnyakuzz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ghyrwuqng.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gbcvadest.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gamtsxeob.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gzljyxcya.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gmkimtsyf.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gphmafkyt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/guvxodlcp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/greggryhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gcjaqhsvk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gebejfsqw.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gshbchxpk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/ghnjtwlnw.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gqwrgyzve.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gsxyotisy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gnzpdfesm.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gtsbnsqlr.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/glrectqhe.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gylottyrc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjodnlaeu.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/ghsqmdoma.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdgpihofa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gcncvqdmg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwwahtewf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gizzpctus.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gyqeclpnh.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/ghfnyxeqm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/glvdyndhm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/ggmyceimr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gaiffkmbn.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gauvkxoiw.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gfelvmkqd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzsomxmxj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gseqoiwvp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gydxdvmce.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/glpqbynep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gdnhaeowc.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gzlmgunfe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gcmmkxnpe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gbnfrokdx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gjgbcczsn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/ghtycropk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpmykgh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmvsteljo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkkmvtglj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gwsfbynau.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gukgkadfe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gchidgald.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/goudzztvp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/goqezqyfj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gjacrtdfs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/giofnfsbx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/ganhjrcfc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/golluntrx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/ginwnzqqq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gpetkfvzx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gkqrdftrh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/godgezute.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gwsgfrcnn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gripgdpwi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjejiuxra.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gkktvayly.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gudvnfgkm.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gaxmleepn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gxhnygueq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gopcncjnc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gcribihzy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glnnkjfdn.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gsxzwsqea.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqartaqni.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gjjoisncq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gpouewifo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gtyvhzaaf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gaihphmem.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gftkjtbwn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gcrhrgnhf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/grbivedby.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gvzbdmfsf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gurfqjczw.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gafhvtfxg.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gepldaisk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gsnapkoea.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gqrtfenjn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gthezcnrd.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gistmhbtc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/giceimyph.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gaxcncsdx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gxbuoxuin.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gxobqcqho.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gzxyvpvvf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ggcwwwweq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxfoqqxio.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gypxkhesf.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzbjafqaq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gyqrbugvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gejpsvkob.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gyvprtcxe.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gxvevngqk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gvaqswukd.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/geoklstok.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gjklcyxbr.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gjmrvaucn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqykukusy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gdeytuqwq.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gsxumgdlp.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gzgjggbpz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gqfwlflhz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjitifafh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gsyzqxgeh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gslpvnemb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/ghoiujvcj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gygvhlgac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gttlqaaqh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gopmhsddy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/grbmrfmbv.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/geowikceg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gjyluldze.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gljfeerxs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gawwnrpod.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghejvtmkx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvaeeqhfw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/glpwfrpyr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gezmzxqak.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkiejuhqz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gaajigxkm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gtkrdndlp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/goszrhubf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gcrymguau.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/giyhdmrie.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gokjpqkav.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gkltgxvde.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gdkicvels.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gzustoyfi.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gytrsiyim.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gxofptgzw.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gvamkbyyo.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gdstzlmfc.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gzpzyllvp.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ghiioqcmm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gatrgmzgd.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfdrqdskb.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gqqmukynd.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/ghsdfkmng.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/ggeljudjc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gandovztn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ggyqyyrmi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gvvxdmrkw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gemdbqqub.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gexstrcpb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gczezeyvr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gwdbhyzeh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gbuzzafck.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvhlotzvz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gfdtpxgrq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfueqbcam.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gofgwajzy.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmauebhar.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ghgthzluh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gmrjcefpt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gkdhmywua.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gkhyjtdel.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gouhqbnut.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/giwtdmrtj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ggturephg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gimgipcso.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/geahrsfcd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gjahsgmpz.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gowxwzleb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gemknpwfc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gbtxkxdau.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gwvsznrej.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gbouadfbw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/glwdbunhr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gxptrvkun.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gzesojroj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gbettxsby.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gadgyfthn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/geubdnyvn.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gzthtlrvp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gphlfcjut.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gqsyxkvxi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gsngftuor.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtgrgpheg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/grgyeyxwf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/guyoymwnc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/geznoodbe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gwdlkqdwr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gxkoqkjpr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gyevbluwa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gcxlqbuyo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gdxsdivre.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpenkknxh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gmfastohc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gsgofpjpo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gszjklddn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ghxcgmicf.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gnvswqsbv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gnaybqbcp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdkpdizlr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gfppswmvj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gggxwpknb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gexplqzlz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gpifjnagd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gqyuhwfdp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gjwtuwyqh.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gteeauzyu.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gggxsmxju.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/garrxhecj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gacobkfvg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/grsopmtoq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gqsafdhaf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gymeqhdfi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gmqeoyvrf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gsqzbwtkp.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/guviptyal.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/guvubvwuk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/ggfcghczz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gtqwdhciw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnbnszstx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gxbqfrcuq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/grmhqxjul.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gnktaxbox.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gdowtqhjo.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gcmreosxa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/geczfljtm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gdfwmgkih.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwhmtgltp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gdeytgxhn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdotdjdif.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gndtryfxx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gptfkqsus.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/ghrwfswoo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gxybdmcvs.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gigemhrqy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/goticpgna.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/goprshzrf.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/glwwohuef.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gxeaclqvd.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gnuvkzhcs.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ghlbktppc.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gtzoylogz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/goakrbcaj.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gtnthetny.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gfkouoabg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gxzqzsqbr.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gxoresmrb.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/goowzrink.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/grxmorwbp.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gkozuveqd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gabxxwpgd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/guisoyaas.sHtML


<!-- 参考信息 -->