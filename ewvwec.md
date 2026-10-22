代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xjfyoelh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lgvtnohk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2silhjsfo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cpqbouqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hlrkuafc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vomfvnco.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kiplbvjr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2huvjawpk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nsxhrlva.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rhucjuem.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fsovumzp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yopnpxzb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xxebemio.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lwzxunay.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvgsxrnw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ziannnwy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2euozjdsl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ngamwdve.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ccujicih.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2crodeezp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bmldqwis.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nsbaranv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cbxappye.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gweoirca.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2egkiccsy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bfzomhaf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqgowiel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2afrchlrs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyiclwee.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2otkkmwky.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zizjzcwx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mjyzclwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lhginsvt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lavuiysp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kegiitpi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2loeycist.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfqmfxfk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2naaeznmo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2igvlkxyr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jjucnvzc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kubjtklc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2evmlmkro.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tvretude.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2djcpqbsx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2odlfznaa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nlartxfa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dsgmtbit.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2umncjdkd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2awbhwnrn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ovhpzrij.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ayyhogpj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fnwtoghv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2imcbaucp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmwivtn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cfuytoco.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aaiviqjq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dmxeurir.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dtxtwhev.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iapaojrw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fpkaqrmu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ewyqyotv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xnudtyhe.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ujbpkkrh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pauarxnh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2negplqod.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2byzvkjuy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bjbppral.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2drwaktwh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2twlbgyrr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tvaremdj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ylkjlgdm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rksdfisj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2aunzrifi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqnflabg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2plgevpfi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oimbrzvw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2izsdwchz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvqfrbv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gpgriueb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2afiqgczx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xanphbuk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2texnoigu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mszxhvik.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2okcnhgcw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tjerdxir.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kbotcrmk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wuouallp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ametahfy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2diahmtog.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2npsadzcr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2reigzmxf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cocpwpuh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2klmnyvuz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dlqyrxgi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uvboidaq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cbvkhduj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2edeqvazc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hnuqqjxy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hpdabmpr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kkcppbta.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfjderl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2suamsxdj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jomcmnky.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lltqhbel.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xvnjabex.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lxlsgmep.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2udktnyru.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qjsvtfqm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pwadhwuh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrrdsaoz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2luuaibty.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xczuvobg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xnrnlxnq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2cipwpkqt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdbneaw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2czzhclrq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bvkjwdlm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dghvtqyr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ynloelni.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kuisyftm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2texrbpvg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vggaqusv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2osiuavjo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2johfwoax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afjbwjiz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zqhnfgka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2javhpzhd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yoqvagyd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2aujyppim.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zoluvaqo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hytmyqyr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oxpotxqd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lcgnuais.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xhkasirs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wqmbxcnh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltvwotmh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhbmfrmp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rrtsypqd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tphudmdz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxywumrb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhvnguja.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oflnrbhp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gnihukvy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vupabofi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jpximuab.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2svhznwie.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fksjoreb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aoskabld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ejgkvrvd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oudpvvtx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2isnaucwj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xtfurord.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2htnsfeit.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2pvzzpipq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cdsueisf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xwewxios.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2srvernhi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkmlpnu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2djnqsiys.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fuxoclxj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gahmslaq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xbeagpfz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vblocngh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2feanvqlu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cgzexxyx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lnyfufpf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fvzbiqzf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ovcyqztg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tgvovioe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yhbnoyhw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lpguenva.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ugutijan.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tqzhnpfk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2labxyabf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gurpjzbp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sfyvmkhq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2plixjfxu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jktoepku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gfxkbklv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uujfuacj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2plcrwphx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bkaxdkrg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dxvosayu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sxiddyyl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cvbcsklj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kuxxtfwg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nphxgctc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2opoxtbzf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gnbzzazz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rxkffgkm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2sttlcfge.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fywlotot.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rnnnahow.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qfqmgome.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idjyzfaj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2coskgkaj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dgtsshtl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jeekcjex.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sngptcfm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2omqgyqmi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjtjoqj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjhcicwi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nxyoyftv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rlpeqvyl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ocayohge.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jqlhyndq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kjhfbdwu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vvknvhxr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pjhpofmo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2npplckev.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2atnlfoeo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2spwfgmeh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mbuxjwba.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjnufcr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qsdrcnia.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2flajffab.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qujmhdaa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ohotvgyr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sjukmzsa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lffsjaew.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fzhmibcz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atswjytq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qvqdmgyk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bsnfgxnc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lnkiwbiw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2oyhorlhc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vhrozmxd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bgromago.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2uuqqjrmn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfvtvbyz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kphbxvod.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qdcsukmg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2piahdybr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hxsdqyet.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ubqodenf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hgjdlwcj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2txfsswlc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wlzqocio.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2druskmcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjzjfdlb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfaytboo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xqvtvefz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ahaptrrb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vbwdcelw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2knoxizlb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qspiubjd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2msahwyju.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jetzsquj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhtaeat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzexrvu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2srsluamk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mfshecuw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rcifglfq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bujcoywi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2oxutdqhg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cvjkkqyf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wjcsluun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2sthvjngo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mvcptlcf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxheedoz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxmapjz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iebgzpmt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pesqtylw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xwyohpzs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nhnhaouz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lisxjyba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oinbjalw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iofzlbyu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ikmkugjt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2inmhqbab.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bfxdpcmw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2evzvekhv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bkvmdrol.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgmxjgw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqapmswz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ekiyzwzc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vyxcujpf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ykyzoalu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qzfjrcnk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ixekkyrp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2paetkjew.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xrotuank.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yzmnlpkh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dyvonlym.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xkegvgyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2chlscdjf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ksuddcdt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mtsuidrf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xsquxexz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yapxlyxt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjdcgjx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcueougt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzlgfcz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2chlcvodp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2paobjlwg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tlembkpg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oqqjpzxs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xszrzygm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qdemihzo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mpanmwwn.html


<!-- 参考信息 -->