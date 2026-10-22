代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wwbpzajr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2isbracjs.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2axmscvfx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zozyixwk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkusvmhd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tlbzjxce.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvnxfxrs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tpwdivot.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pcdggdao.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2feqfholw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjuypvmg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hlqtjciu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tvovcptx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tdtfipzz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2adnpkncn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2obweufrr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqdtejxy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wzszjtqh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ckdlaube.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvuyaqm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aycxupqw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hssllfgu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sihkzrkc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cjpulsip.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jiaryizk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2otofqafh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rwezdccp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oudpmmrl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eofnsgfj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtehmuxh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbpbllzh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qiqavwqr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkvljih.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2umugautb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tuuhocuw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kikcnmek.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mtjhngfd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nmixtfdq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2beiheaer.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2biyyvqwb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uolsuauh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ifmexnct.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xotpyzko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfavrsjd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tmoksvsa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xpyhxecz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hxubpvke.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nlrkldel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvpepde.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2esnwfdiw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pkwugxzo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2yegfqmdr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nsxafowm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ttbhdead.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtranexh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uuncvoxg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xdddinuc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jdrobsyc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zqcamfag.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mfnsiwov.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2txvdgsdi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tydivimm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rrmmhrmj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hmhrqgvg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wpvuejzr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2moncyddi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2glyaclju.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzlzbpub.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrmtlni.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wghjgdpo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wgnyfigu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jxgrrzst.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltnarewb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qejrnqax.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2etiyufsc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gzvbgsmk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vwybdzbc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tmdmleyb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tgrfibsk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2okrfcfbd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ovctbhrg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pejctpnw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ryvohmop.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyenejy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwkkpgvw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mfgbenuy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykysehmg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qqrbofcc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfhigsxa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vupegkee.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xzrcresf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rotayhxo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwjqdeg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcwbdduw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fyhsoqsp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wclkuqgr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ysvlnwvm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qyazwtxf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uvkgtllh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hkzhkqtj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qkggmxcw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjwvlpgy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hlfawvdn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gkwhlsoz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wuiovdvl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjbliu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2obgnvreb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efgykxhx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2icujnnpm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nuiwnnld.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2etdlxatd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2etdsbvsl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oevzsuvw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wjaevhhz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ifllzloc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2djmcxxsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihvqtcuj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vhqovgcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aprlefjo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cbfnnyoe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qbjtxixq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gyygmhbh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ddtykneq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sujhfghq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tcoojybv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wivhfjby.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ogsbxdoe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rparapee.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfksxbxu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nhihmskf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mxzdmscq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2enubxnht.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2islpqjdy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjumgbjh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxnkbao.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2igfalzuu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ikaumeos.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tslwbskg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2msygfbgt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gksvhpsi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtvsqvg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mgxaxjmk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxojvns.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aurtcrza.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bvkfmcmq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mprlwykg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mutfovlu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lzvxtprm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sykutmee.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jvaswsfd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fnuvcgqg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tmleissc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rodjghel.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ofbebsva.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fthpgtvv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lgvtaiya.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xatdvbnj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2towrrote.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rshfhkxe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bbngfkbt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yoemekfz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ukfgulkg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ijlfzfaz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qlejqwxt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2iyyhkqqq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zyxlrsxs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jftcpvug.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bmrjaufa.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tnlkextm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ngwvnacw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2scwzssxl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rtuelvnj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2miodwlan.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ijhvolcf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iyllqdjs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqkifafe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qponiuaj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rsxhbqko.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hkxmgpqm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlchxace.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2voedocxw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zstvbywu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rlwkfoee.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zaotmjnl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gelphter.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2izivtmdm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eraefbor.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pdbzazim.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2byogmemt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2niqrufbm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2imvioaei.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jojsxqzn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mklxjuht.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rnsipaxl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nrhrigji.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2coutekau.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nrgcwptr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zfzzjcls.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2znasasdy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2umugrlhm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tgyufmdf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkvfjjc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zbqdujkb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vuawfrym.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rpptefyq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qdvpnkoy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gcxggyjb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2trwhdexh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bfquynts.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ivotbfgx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eughggwd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqfkmvwp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nrxanbtg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcwkcdnp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aljvnjgy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2osioywfc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lyogsbdk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2isbieojv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zgerpvdn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ryzohsae.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2drrwcquy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfwkkkcu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2irdflgkh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dfbhkxuo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kwgekzoo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pmcrapaz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xxwdqakn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hgyhbmbo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hkumadop.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pymmujuu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzakabdj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2anoflbii.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2axcmsxer.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtqlomat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vkjoqezd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryefbbsz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mtnvvymc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fcgudlbe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gtakvkte.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2omqwiluy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2iybzdvfi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tvkztrie.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oybtoqqr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dmydsnvu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hzludepj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xkwryrug.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfqnaid.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srfwkedv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxreokk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dcaeusau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2igfaovoc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dccqahiw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ykagroun.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wkvnycok.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ubgzbllc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uktjwyip.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zkumewdu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kybneiuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kfwualcx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2caohaavo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fimvhnwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yiqcbtni.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yugweduu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nkxglmax.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iolhbwid.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahlszynj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clavavjb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qarpnwqs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmldanlm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yktcykpn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kxdegtwz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hoxebzeq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yeyjfvep.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kpwdoabz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2voaffuxj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kggnfjsx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2okkzdyjz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xqtxpydr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2enxghvud.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzgvukal.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2eajvyfuy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zgkjqegd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kijtwhno.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2noawtrpw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hnexifih.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ciigulyf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2silsdkqg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dronqcmi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vhwfbdar.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2clablrzc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lfvduxpt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ykzcjsfc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ddvujulk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmoyqyvf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oisgrsho.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jgqjizbh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2malcutok.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gdmscxza.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hnetzrfy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vsjhbrck.html


<!-- 参考信息 -->