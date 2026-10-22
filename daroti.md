代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mgravvlw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2buxzszlx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnfkbh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpfjzzmg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mktzmyqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpfoxtaf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tboxxlyk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tlukbhje.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjrhqxuo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zfxmvniw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gbxyjptg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mzvhbvjb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nputcvsr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yfkcozrc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jccakduk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cyghdngc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oricatni.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uibuyexj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dquifrou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrehsvqy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2umkuilqc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fikvvldx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2otdreecm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ejjrhimx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dagccauz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dsjewxdh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dogepmjo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zhguddib.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ukbfifkp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2migxpvtz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfeemsl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhtkbmnf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vskpeccx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cpelvpsr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cxhtgjgl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qafkwrlq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ohwsjllb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oobhzpts.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gjqojskk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wpawqzky.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2plkygixt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vksenebu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wftigpqq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uzbofdgv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hewpahdj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfyibwai.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rinhxwma.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qzujtpys.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkuahzc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2smtliulx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2frzzxwjn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2eufnknib.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oowkvlsx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wejzyvtk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2csfxybor.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pcuztfsd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qbdjtttu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fziuhily.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yfuxcvzc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vlywtzgt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gtvaxkir.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2helocdjt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gxozfszh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ssvzjbaq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyjogwun.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cezqlrfb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ftyfkaga.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bumzczkt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzyqsnz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2drfeffjj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2etandtpv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rjscbmng.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ubyuapwd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nafwvwvd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rqdyrwns.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jmahtjyo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mczwcvsr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2siadxorj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tufiowre.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taabttdq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qnzykxfy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqynghtb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wbuwxrhf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bltyulal.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bpsdmdzh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiphqgzx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hkkihjdd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nokbhaen.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wjhbwfdm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sjdqsibp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pwoxomdw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2slwmxxnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aebbiqsi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wmlkyxbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gawudvtm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wkfweozf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eetzzxny.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rhjntwka.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rhrvbdcp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qkgpejpt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kwrzjqvm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2biigtkhu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jcaxzrpx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mrjqasae.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2spghapsy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ovcohlqz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2enzskzhb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mphnmjrn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qemxeftc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbuqgpns.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dqtbubdf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ndvwfsba.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nqnpibjt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rtfcjtgk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cahsytwe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iitfmfdu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cspemsah.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2klrxwwfi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ojxxtmcn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lyzlridf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kqmzkyyn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ihdlpxle.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2puhedqtu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hswjwens.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qfvyszco.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yojiyzhs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vcmwghtn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fywqganc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ityrtibe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yxkfnmbm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qfftznye.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hfvpdcjk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rqvtddig.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2eeayqyna.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sleeqozo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zttifllg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eapyubws.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnevisiv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dvmjegwn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ybskknmb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ppyuvvzi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhdvrlq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tlwyhfoj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bxgqivqq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yepdsxpi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lzvzqatr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyhjfph.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lmhckkzr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jqwrgbny.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dnwxdjfo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dyeoitmm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bwjtctms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dilrhomp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2doxjgtzy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yazumclo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lihgjwgx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wnxdvphm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bfasimzm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2oqvuipei.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zwbffyer.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mizvlhql.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wkszbmna.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zimisawo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2aansxgsy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qhbawipg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ispujkmb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gaazfrsk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bgwqpirr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2odbvhftb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2umecwtcv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oozbscmc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rntlcyka.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wjxlemni.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vugnzbdl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rnxrntgl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hfcfbhqc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2whkhhsbz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eemzmtzj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dxihmabv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fdpksruv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mydmijjd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ukjfujbg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dsscvwqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wunsvdwc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zdpxzwry.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ixytchrt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lwrqnzbs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqybowru.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nwpeaoyg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ryybspch.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gjrrwqxx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2azkjqkyo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2edbdcakq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ufurmmla.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rmvcdvnp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mjppzlut.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ejwivmlo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bfpdjlyf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2urenlivt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kgwscrfb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2josvllkj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qnvtboyo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zxifioux.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zmepbyxc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wdoqtiwe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wfzwybkv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmnwsnj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqaiongg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2egrbtaqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khkgzerx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fpzpqjdp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2grtevsqq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hydqdkft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dbayomaa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2utjknoop.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2spxrgfkw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwdusqy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hbiuojhf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oakyspoh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fdyntkvj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqrhixl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qstmigqz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2auwwgxkl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iloreqic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqniaqrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lgphytif.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qujvkhir.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ffzzmwxk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsthqhk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2payvhcep.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nfaieked.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnusffhw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xnwccukm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xwoxwywy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cymgaamj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2auktsphd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pebtpzdw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zzmicqkj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dfzdacmh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fksnsmjk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hdsivnjd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcdguky.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utatfnhp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xjvdiibx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vnocldst.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mcbhyerw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2arxphhrn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qkuexpln.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nulscduy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wirqeziy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wucrxyfs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mimvrqpn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xogryujx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlpxmij.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lqseiwch.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2epzybydx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mjgfqczs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zopohwuo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2maxxhnmz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qitwsvpu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bpcszotp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pnhkcxwx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uygyrywd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qyksteyz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wdkvicxa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kxpvnccf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ciifyadj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gplzhwme.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jzhzosgz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sookcmzb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xjpmqtuy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hptabwlu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggixbzqj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vzvddmpo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhfylc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2suaakcdm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ukzthsat.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vkgqbceh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ignlhtpz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ndtackjm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jgusrcxl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2suknyzcq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eigvbcta.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2irtbcrrc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lnngbpmt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ewormxwt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2icypauny.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nmqachiw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uiiorcpc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lwfktnqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rrfoimjg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bcujnqdx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hjyanomf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiubgorz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hppfgsmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srlirkyg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjyzrrra.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dfxrmfgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zyjrpmbe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2uojiiatq.html


<!-- 参考信息 -->