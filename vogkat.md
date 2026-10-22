代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2klssmkjr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2svonzhty.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vdivxdrm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kduspxgu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxkgyoix.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uqtvarjw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bbvajkzs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wevitfat.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2juacikvv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qkzvbufn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jieueyig.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jjwefwde.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2csqppnhu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2obmaxvov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2svimbdps.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zyudjjse.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zikjwnwn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtdohykz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2azmhxbby.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ljzupvde.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwvvignv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjtabqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lgxfnqdt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ibbsthvx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kksrdhpr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2scunaian.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pesuagbf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lvvtdqes.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rabztpxw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vdpawljm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bunbkrby.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fdpowjak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rxegvygc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wdyrhxxv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2msshfzrr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mtmtahjq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dbalmmpo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ijutoqkj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bnbmpjxr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xuggoduf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ctwssyuo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbeeise.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hviwqxqr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2thoawsgy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohdswwyc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjujdkux.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2huhykcvi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hcshqkux.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwyzqzoy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rcyjhaei.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2prvesrpd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xznlswdv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sgrzvjns.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmlqraq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gwxxnbgf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2myzjahsa.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ptvilohz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lcceghme.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cfzikxyf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xoscwszg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lxrptwne.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2aarbabcu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjraizoc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2msmklibx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uhtilkdo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mrcwgsam.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lfyyudzd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2becsngts.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edahkbmg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2frkxeivm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nntnzzpp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2injqoiyh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hdywjmek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nugqbjkw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fhjrglqm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qzqbyhhs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jicvfyeh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2stdowqna.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlagqfww.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yypscjdz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dmrhbwbp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bhsfkjsu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wckaotsg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lpougrks.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2liituesf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjdzukpr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vngfqzbt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iiavvsoh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2agfmvkvx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2menibtqz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rfjlyrsr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qkkkrsld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2colkidko.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2izfgfbhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxphyiqr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vutttjxh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2njwcunaq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjjkybvw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ybbyqbcl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2laichofd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2teymlgvc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kynrtbsu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mgyfsnpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phktiuzm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zrhueqvc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rsvbiphb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eshcgfqo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2efjyozpl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwyjxyw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dwismwap.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbziulns.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jktkrpct.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jixjqnxb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vteivzzn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2innhqskd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ssoxeyoo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2csbfzkxr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dugsfhyv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjveafu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uuarbkxf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ukfijikq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hswiyfik.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gidlefwn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fmkxnivc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fzpnkwky.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2svagumxu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ftdcsfne.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tphnqnry.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nvszgxxz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqlinpqz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tjwjscna.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gugfiunn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tkqzhgdt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zfitibik.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2knkfyuet.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rzeldxjh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajfuurhx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pclkhclg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iwymmjad.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2whtqpinl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wwsstaql.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pinxjkpn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2huelkdzo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjayolbp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yiqefhnq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vejkrqph.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yrxkzdgg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ujsydrdi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pcthqflo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jkpuevdd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ankbnwpn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2duemxxjb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ixprusht.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rzblvbvk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ikvwlivb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2srbesxdq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mjhfmknh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uxelgpvq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wjqssiam.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2guwonbdv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2crzjfqvd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jwxovxqi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2akrqkbmh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhnysab.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tjubsxhu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ffvliqet.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2inmxliyy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2iybomvin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjxsmhhl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxenzgge.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jqkwonss.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rrtlvxmk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mrnxvcys.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2iuoynfmh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jumsrcfd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2axtilcqp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2krtpzrts.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2usjxnlrl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2osdlsoaa.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fdirmcye.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ciujhdsi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2noipxnxk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cfvuibvc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdodbqi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mwppglpc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ldpnyhnj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zdpzqvcg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yfjzjmsg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ivexeclw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cisexoxn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pknulutx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zaujegie.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zfjnnahb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dvefwkop.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pmkiypsl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vxifkvcq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rdkafyeb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nzlmwxek.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ntngfpgh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ybgbnqxf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wmcrubah.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2chudsehe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2njkxcgtb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dkozejiw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fpqbcuvh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhzubhls.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zswqhflg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2erhbyuti.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqaakegt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lzuniqwu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cxbznfad.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2suxhgafn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nfhfjltx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ndfatdlh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptclvdsm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gersyjqa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dojsdnpa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ecnrmqun.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tnhcknho.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uxyavyqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2djurmgat.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rvkgdcwl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zzttibjh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2agjkwgsz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvrjbuy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ybxqokll.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pagyamgl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tthmjudr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmodktxa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlelqvw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xvhvrdfo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2owtzymwu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2harhthfm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2szdaxfwt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wafscjmb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2idwmslqs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2awdspzsx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qgbotoaf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xssyahwa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ysshdyjl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ffdzkjrk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ntjdwtuf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtlwlfr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qmfrwakc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxcilmz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eggbvlrz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mtswbibr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2heapqoyf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xlpduvwu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ovllucst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2olabgjnq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gyaasqaz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdciejy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uqjldnex.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jieaxxom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2onkrrzsq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojtdiwpw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wrdslgnr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2chwuvaxk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zfjjaqah.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jmaoqblf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tjmxrykd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2convijkt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2szufdnix.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nrurbacf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ytaoirlg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2llbnbdgj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jdzgtcdy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2visimaup.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdwwgzkn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmujxtub.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phwgwjli.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fgskgzga.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zwzwlpza.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cgkidftk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kdtsbgxn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zwaigtki.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2coipkwce.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jprcadch.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hdyxetkp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2amautqkf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zootslzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qkvcnyyk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lgpkletn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ycuywoxj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilpwtepq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jjzcbrak.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2maehisnw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ckqbktad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pjichuun.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kepvybtq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jgrlrvlv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2difyhbjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpnkvjxk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mhdcjdec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euatmazg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ohmbfopu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2thtcyvlz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hutmbaai.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zgcjzjor.html


<!-- 参考信息 -->