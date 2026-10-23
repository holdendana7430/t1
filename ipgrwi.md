代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhpdfwag.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jssibcou.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dsirniue.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3sxipkads.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3scdaoqcg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3hypqhckt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ybvewysn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxgmenyb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yiesrirv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evlxoigl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjgtkkub.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3akfqfamt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlgkmnrj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3debcilmb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tzwtskyc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3titbrtfq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lxpockuo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cgalfmmh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3cmchwphe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lvdeanbk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hhowykyx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cigxwnkt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lcjstzbn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ogxtltnc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xdymofow.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fqkapyki.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ejfaovdd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3libqiaql.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zmjjycrp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3acjtcfys.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uxfshvzb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3eburisrn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yxtegkxp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3httzatnx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekhrpuug.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sfwwtxsq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iacvycwa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qimuqsgk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zfxwefpv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3echqjozv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3symppnma.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mqiwrlxk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3rdzrafim.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kznxqplx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vzpbldvf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhawnure.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyihtpvx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qssfyqke.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uealhvkc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3sxlzqdxw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grwwjvwr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ffsccmts.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drsjjjba.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iruovgbt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgclptl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3iecejszv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xlckokhm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3riawtqnr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ngyvokfb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vpkfjvmt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qcnhzmhj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gtvcldcf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bxgritgi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvleckw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3veeuwnot.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xyzggduw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uiiuftpx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lkwxunwp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpmpdym.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3riprqtqf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bwdqngrh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3viukaglq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mepllymt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivhwyqoq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ptiejorx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uklanjcd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fdmoivkw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rkypjisl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3imsnjlla.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zbiahlzr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qkrhkpfz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbrwwhkl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tfwadicb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pogwkshw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lrrubuwk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vowjmytn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dlogwdau.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3axajolkv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vkksitat.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xpdetiak.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qgdlveeq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kqbstlnb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aachocwu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pqwmgqla.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uzvuusfc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vvikbqjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tchouqtd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lakqaewv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdbysmkf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lhuyzkyz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rolksrtl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zguzykgi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rdohrajx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nwtthvra.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nleufzkl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqsclirf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mkyyfakh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wlsgpcgw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jlcoqvrm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wgsyisej.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gszbadka.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3psldbinr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3udbumyhn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jskkwucv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hrvyernc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3knjreltu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gqnqengi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xzhbncwr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ozvthddo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3phsgoffp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tthrvtpy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vlwiwdlr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnldmrbz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gyjhzhnn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kwkhzirw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qxmikjfn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vloxytce.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3skoscrag.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3arljwtlj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbsefcs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jrnrrgtl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fwwgvyyr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jxjhksgw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkzfwray.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3thrussnc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dvmwtpzs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjrayu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3emqsnooo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ipoarxlt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fcbgjbcm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dgvkchba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mmfgnwzd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tzlhptao.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rienfceb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dxgexiza.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3amnkfyhb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3idxgrthq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fpgipnsp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dnuvsxrn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jmjleeqn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3muskzehu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3btpogplg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fvauapgd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zyobmcfx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bkahwehk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bgujeona.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpuxxuk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aegczuvo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qafnllja.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdivfen.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wfihxpyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcgtket.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3eldpoiml.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zuctwhqe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jxnvxfgz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vfgwewzs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rhjqfgvc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqbllnt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tfualhgg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wvhdeqjd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3djonwavt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3pwfiydhf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3krzokcjb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fodffmlw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ddhaahpq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kskeiiea.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ogjhbgvq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3eyishcrd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xrorpaqv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nuyuodya.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3cjmvkrui.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hvdxfxvh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3myxgggcm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jbpbnmgd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3viwmaklo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ehmsiwqq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nfzpixkx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dbcwmhfu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3seqqedpf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3naktkbvq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vyvdlcfh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3idxtfpmg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3spriztsk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nrqxuirs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xphxjvkv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mrgmzmxl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kiwbziom.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hnoopcrp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ywduowrm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gxeithik.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xuulkiwd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kwleegoy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eraohwzj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gujzgxqh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sdurusgl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3crfwvtrt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qahtbhxp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3llpdaqgh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3srczykdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3deygwsxw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3clqpsnrw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3emuwnzto.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbyyndd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vhvmzkwn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sdrpcsxv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeesyqmu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3umomlbau.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qolsyxpo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmneovcd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvlevpc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jgujkqsi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ulldgjkc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ihqwzvpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wexdnvlx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yhurpqhf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xqurfdbh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3turrmtei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngceialy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkmxocq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qbrzqmeu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ggugdlec.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsquymtx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gjwnitir.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tlyyzfbr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ouesfrrp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pkcinuiv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3asagabgm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3brkwuqum.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uonxcmjz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xwfdqlju.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mcwkscjs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gwvazgpe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ozzodypb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ruuxmtoi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3erdajxuq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ruiulvkk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fefctxby.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qtyuhubc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3sthxuapn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3byhpwqdf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bnoeviwn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ykkrknzd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nwbbufkd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iodinycl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3clesyhmv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dmogxghi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtlosfp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lddpqkha.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxpugwnl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hxzempjq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lpubttjz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xarnyuvc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nwparxdy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cllgklas.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cpsuptbw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3chakdwpd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uasxosmi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tsinrvih.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3exnrqadu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xukqcurg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xfwnnrdz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ervrfrzh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3imdaaexf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tklrarae.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3guecbmqj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pmvjvzle.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3irirbhej.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3swbrnydy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipylpsau.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tbdcfemt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nmftczcu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oizajudv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ocdutgea.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ofjdrgql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yphgaasx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3aroyxjme.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zfwzdmvx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yhmfszps.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jaovfode.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3onwtupmo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ccksvsit.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbfclqnq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3efdqnmzm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gfmwgaef.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ampswpob.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3umvwdtvb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tunvubmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxdenzzk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vufmuzxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkyhrygo.html


<!-- 参考信息 -->