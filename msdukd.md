代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wapofref.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3phwmdqfy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oolimahj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3npdphjys.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bostcqev.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3axxusllq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3igygmrad.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sxgggibi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fpqjdpsh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ljgtpito.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xthaxpfy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hmxrazba.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jkrvtxsp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgqfxeg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ohbaifca.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3osayuatz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tlfykpot.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xicywpzb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xwmoqblk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pbcukqjm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jdboybjb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ppeucriv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzqtbvox.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yjkrqmuy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3adpekpzq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nsoixayl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xaslfarg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xvgplfdr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hmelavml.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3urnigyhd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3rssnlhml.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nolrkywb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ywkuqqly.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnbkiqa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpyseups.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3copjpldn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wafmfplc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3doaoheim.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brvbxsjo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3iqqfczgk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esqvrhuf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nhyshoxd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojtyfxai.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bfirmteq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3czfellhn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yjyjhefw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ktpktldd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wrbwjbty.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hnemikxu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tfsaralu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jsugxptw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aesyiubo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bsaujdmx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3numxheze.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jkvalshr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nclmptcz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lbychrxg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rmbiykxm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xmsqejlm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jabxrcyp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ukcuiftw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cuxqgaou.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vpzanvpc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kcknxptj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hsymlbju.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ctnssiob.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jiksbhzl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tlaewqfn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lguxatvw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3yglkbovw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fhryrdjt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zfmnkitk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3aqkgjztv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ldfwtrks.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ykyrvasx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hedshesn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ncdmaxvo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kpoyhtja.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bdpssyqj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ciyifzjt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mpyziytk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hluoxbxy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbreyiza.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cbdvdlfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iabxfalr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3okctyocn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrtoajvj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uyktlmup.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nwkshptw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fatkcjew.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wtnnwvgo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufenlidb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yqogilsy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjrsxemm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zhdiaskm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dacbrnrv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nzzfdxiz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ciktmovh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejtknvzp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdegmwf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjrhaxr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ozdkbvbn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yafkguid.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xvvgcgjc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ukmcalvx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cnzdqjpl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xiqyknff.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3citpvhqs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3swmsydrs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dmfrflkg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xpzkxmod.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tqhcjlfc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3asldqawd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3amkgfqur.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ytemmceo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3slgdvytr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3grhuhunw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsbejyk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gchaykli.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zmryzazf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mwymbyte.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fwbqdlmw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lhiwsylk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lkvhxeii.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kwgztbrp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xqnxcttp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cnbdezvo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwohdux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uvgjdcuv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wdsjhift.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mfpsfvbt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qwbcmpch.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kynptmgk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtcisvjr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxxmfuyn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nzvqomaz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uamaoiqf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xsqtydmp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3elpigfeh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvnombzc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqlqckea.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3unpgivcv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fbxejbqp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uylqfmwb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wpeckztd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aiwhcaot.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3avbewhof.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmeventg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3huujdday.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jdfabhtf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xjxctzze.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dbzzxleq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wframacy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ntrpvttq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yixxrzef.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vfumtegv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kkxksvec.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xqksgbfw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lbzilena.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3byjmssjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nnkxfzhl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3izhmxoiz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtksgza.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nifmhrlr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vrdayfjd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3udehpfpj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hqtrsiif.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kgderbhy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hgtasixz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jipitctm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nakuzlhe.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjxxsmh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hplnzqlk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jmuenfyb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fneopell.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xjlaujah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ehvonliu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xoxncbgd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3deiazxky.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkkeplli.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xvwmndxk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qbasmgbx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3doabdzrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hsesqymq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xrmzfkxl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zemmjpco.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3krwjftht.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ofuqxwnr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gpvxtvfm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftjwghgx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eytwsumq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mjwqhmjs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3viwjrjer.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yuuwtnvt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kibcqeyp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3szyjdjfo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cotabykt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3prnpyaww.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3azjjfjkc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufujblfo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngiqnpwi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3brphfwbj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3irkwrhjs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwchksg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rhlzsmfs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3agvrgvxx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ilqpzaqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zvixeipc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rymhfvtl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sdizgpuc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3trdndbel.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eenytnwf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3orgyokkm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bfpxmmud.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yubdqwaf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdulhwyl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nomdrizr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bjabpnlp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zhclcvxc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxaiapkf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gfejrfwx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3duqcuzsh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hrscxcwk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3afutbhpm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xhzhpjdj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3smideiuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rpemuggp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nmjoxpce.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pxeudehm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xkkwhkcp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3sepsxhwc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pntgqxau.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wxwcwfxm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3tyyietxj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dubjjznf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3upexyrhc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcpkgmuf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bpxgukud.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nbzlpdcp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3akvepwoe.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rvuyyoes.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ucvlsogp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gdbikffs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uobchzgl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3esfwtleo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lfgwnbkl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jmtrnobd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gkwxrrqq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vuxuafbe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nkdkdprm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3abwfkzis.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rblownfd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dyvyjaao.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3unmsevag.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3evlrosty.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jdxzrihs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bapfbtzv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aaehhuxv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ncekjoyy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cqjprmeo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tasraapk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvtevbrh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhqajmeh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dvzniboa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wunldygd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rkruupav.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uoaeedyi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tdxpqkec.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cntoxcey.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gumxexma.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kvjrlrfk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nfynwfij.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ftepuovp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ogwczylb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wmrjlxht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bxhfhyww.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3trlrjeau.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3umyqpsas.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eicvonds.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wxlydvhn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vmwhiawe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nwyrkcyd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sxnpoigq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aacelyej.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qbwnmlva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enhkxjca.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hqbyggtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlkipzpa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3chvqtdbl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lxxctlgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qufkwktp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tqfqsner.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3amhmtbxu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqpveqcm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cppfqlup.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vulazhee.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mbdptkfd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tihisfpr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mxalgenn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3avdiywxc.html


<!-- 参考信息 -->