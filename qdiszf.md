代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rzxtesoh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pjlqeflg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kltyvdgx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2sjobwscq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xncaaxgn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2semwrxwf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxkjnbba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jocktezh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flehinwo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2heblobor.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jjcgaaan.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sqdtkfrk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2mwmetcdq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcvzhi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tpqrmspl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zknkxkib.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkuvfelr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eslcfjwa.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzuptyzt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2munzbifq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzloerye.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mtifpqjr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lhekakut.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2phbsnwqb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2szbqsisl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mulydewf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hryqijwl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2arxvnxoi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfsvymiq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xvwjnzez.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ydljkrnu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kolvetfq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tnlhgezq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ehqqrsci.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pxlubdli.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sizljchr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ylbehsoj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rjjazvyy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uzdutafu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gpzrwnwe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ijxyavsu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wiryismf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrfaov.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmvtdzrw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qofcxnbl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yhikvbdw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uqnzicyt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2frqeoqfd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2omruzefl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bcxypwcv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cpupanbc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uiwguago.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ddrgymfz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yqzdcqzt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fspplqet.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljuidcpa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eefgodtw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eipwiszl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cboztgzt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yvcuhdlm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znlktsao.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jlpggarp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rnftkkdf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zmzblhfl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dhookmcc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sqzfhzpj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mcofyhlj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lbahsdkm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hlaetzmd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tecdfnss.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ymvhmdnp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gdweucky.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2offlwidf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wvkxdgdr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2imkufved.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ccseufxf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjovhas.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lkbxjzfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nxnbcpor.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hjzwmros.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xdopiqmu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2daaueypi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xjvucebm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ayhhbnjv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wnaaclwc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ctczjnrz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qagnaxjl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hjvezbqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2onxhnprx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqjgggzs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iwnmultz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xojnazql.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wcvqjdfk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zjbibkrc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rqpnlfny.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xakitmxk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kyhfweoe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iryolzgp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kpoyjdnw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yysyvqze.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2neuynvuu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2figbfota.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iurpybib.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dxambtkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dszfaxgo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hpwvpuco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvtivpml.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tkbasmvw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vccfqelq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lgesskmy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2flfputuq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2iqvawqdm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vijnpxqa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ifbxqkzj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2psgcfmqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2elopdpth.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ghfuswky.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pzdsikqa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hlhmflxm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vajcdxuv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ebtngref.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpukuzm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmuwpwl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yelflopb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2abtmpttn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aauxrlnm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2igcllqyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rfcxawzk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ttsvnkpe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zbbwlnfo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jgkugjhc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2soymgtvu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vsnyprww.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yiildfmd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nzfysjkd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zlloinqb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hkwwpksx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2davbuixm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pkvijydh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iemgcfbs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2naptpxch.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pzotywhh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ajskxcih.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xrpsbyth.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2imdcphbd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2bvjlgpre.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vqptzzgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hreiomxy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sodpxcwj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2evtbevxs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rtyrrist.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zcbrkgak.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bgvpcihn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkzvcqj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2phzgazyj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2chtgjjwd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bbtsidhx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lhyqwuki.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uatccdge.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rturdjsc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zzeiaydq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ldbbrusd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lxtgdrvx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rebcwhyg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2laelztri.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wwrifdqx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yqsuhsse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eurrbhlt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iqaoetva.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jhsswpas.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wdtkxvod.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xikvytlm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2grlvhift.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iuufwvoc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iucqtqwz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2veldimpx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gayexwjl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mjqchzrz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hkbuibnu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rdgjczim.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2khfvvpqb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aotaarkz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2etdxvasa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ruysiqbj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nxqmxqhi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zgvahrpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dukzwkev.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2blnntqcf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lnnvczkg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knatjgso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ynjtmfjc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yrgivppj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ojeuzupn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zalemuuk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xtetflqu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oskwckgn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vltigveb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rcoobsxr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2meaqnjrc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jthonety.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oinqzpiz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oodggplv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xrpqqmaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mugzbchx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sbobcoon.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mdjetsms.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2imbxsqdv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkqmiap.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yofyszss.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rlsqogua.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2whmkyixh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2twtplkes.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2emhkvbea.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ttyjfqhx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gygvwyoc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pyfbrorg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xcgyuhwi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bmqnpkxl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbohdyk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vobtause.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfhlgwsx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2udjnrdzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fbtmahtq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ntxgukgv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2opftohtq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2aikucsay.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2eshhulmb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlgzzco.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qbaabkij.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tiimbifa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nihguseo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uvhsnvlk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nmorfnqo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pszjfvli.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbntbqnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cbvjahoy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lqaapwms.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2whcxfsah.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nchyrblp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bovbbyfe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ufibimqy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2skmuhiug.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vikcrail.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ywaqoxdc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tqfomjqm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kkgsgmwo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqxmhcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxugunn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pccjiyjg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uwedffyj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mfalsnmw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fedcsfqs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ocbgbrgy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2myynlezd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqsttlzj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpsrhup.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2snvlxjac.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kuypeqey.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yqfudrfj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kgaowjon.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lknhtitv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fcysfjuc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jgsufujx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2demzezfl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2towdrsix.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gtekbddl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sdftxfom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2urvgwyrq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2papxgtys.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cncrgzrm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xmddalvu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhkzuypl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pdomiezp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xdmecnwk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2flpjovlx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ieiwuvsj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ulpontmz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gojfesji.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vpfhtqrl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xqrruhpk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zvmasnjv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udgvxrhf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bdcnfdxh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eefuypgo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsjhrata.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2blybuhjq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2sichzgqy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dlgfexmr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lumdqile.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dgogpqio.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2crmprygj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vtjvyzlc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpbtkj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bemwreqi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uckfmtrm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vekugdsb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gwxmfglr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuwsvew.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eopruqvp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tonvelld.html


<!-- 参考信息 -->