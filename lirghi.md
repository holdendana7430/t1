代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nocizmgi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhuzfuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hpwefiov.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2whplhmmy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eugpdrbi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2eluzsjgx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sybodwih.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2racbkihq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2pvyhaqnd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nskphdxg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mubgqsmw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbcxlwfm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zhbaikbv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gkltecyw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zhyjzght.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ciilmwmf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2erzuymde.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2idzlkcqs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dsrragbj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eftxizdh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jkrjfmco.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lorxqlem.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slvlwcmb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvkurlhi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zzehdkaf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qyfjmobb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvprrrs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2irbwradi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrstcfyi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2asotdgjo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdtcutom.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jzccogqw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pzddvgze.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrktajk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gflmskjz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jqgvqzqw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jslwfoxx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yuusmoss.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lefwuvti.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hqcwvppy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vicycdhg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2molkiujr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vxvbyojb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ymchpodl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2itsbotta.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vwqhneko.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rgieqxuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2filvjnga.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2reixmwim.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qlooopue.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ulbclefc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2oznywwso.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mampdisu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pzkmpzfk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2szfalcyv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vhjvolgt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kypfjrvl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2eljmgdmj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lhdsdsrg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ekprsmbh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2aqvbvjqw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhuwosma.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhqfamd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xmvtbwjf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xiyqiukl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jwkiziyc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mypmqdhy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yvvwpqmg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nbttrwei.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yhchiafg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mrsxnrso.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aoowzdao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkgvrjlm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2orrxmfwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qftgghey.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qtclzgci.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kzpxunfw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihuakrvb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2imnhqvvw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rxmmifqi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xyfhurgq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2itmmpqdq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tzyaahip.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2syyrlhmi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftsoqcwl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lvcleacw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cfpwkuzk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mvczqknn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gypzubli.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjniqmx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uolxdpgc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nkgoqwtc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pmfczmff.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ijexxupy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lqogtgrb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jrszjanw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fnkyqnua.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwtjwslc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kvpyktne.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xgkhennw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cmycldgo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rdbqemno.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2scjjxzvk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gehydwag.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qnxvzqes.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2awirulne.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ealuefsh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fnevoshy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nimmaerq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ohzbnvem.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yogphnnf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zydzbfiw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nfexzvbc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2aieoadrc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qjbdzlgm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ozdxenjd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zwfuhpuq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wtmssixh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ojrooqrd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ygvndpjd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dmbyqfxs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jkrbvjmu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jsgapijg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zslqwtnd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xiovqwvo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2crkkycbd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wvovrnbg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2senksazs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ybonbomr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rpgkbgle.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tpekhejc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tebweeao.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oiioqpvh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jtwsqquw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uzxgcidh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2chcjsfzh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pgffaecg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jyrwyxfp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yexigoae.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ujmjahuq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tntciiqm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fibfmoyn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bkwgjzoq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjxogba.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pyzjsqot.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bxiscgbs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ftxplxnx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ncjiakfz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zzlhhhac.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vafuaymi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bkbvoywk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxyprupa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wgfafuni.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2miqbqygr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hjtifesl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kilecwtu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mmjysfzy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pcgddieu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kielcger.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ywyapvqf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dozfqtoz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lyvxupel.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2arrzyxrm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yjwqxlpu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dggtqrud.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2morbcyup.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ayzblhxd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hbqmbxpr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvfkyktf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xidxkeug.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cjgbcidj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ntcmdxku.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nthnkqkq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gkeupwko.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zpjnahnn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2inwfogaq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2exubjldx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fmkhlcve.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzkxtrmw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uyswnnnl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lrowksdu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xplahenr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gbvyvtwz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uzxvtktw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tbgocntf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2brrzuzlx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2putwxgxd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sbtvisxr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2onnlwmtq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2patdovmv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2amclmkjk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2olklhatr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cznefnek.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2okodxfwq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pgpykiir.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ecermvyw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zmqyfqjz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2auytgwjw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yomgkevg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ilahpted.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rjkorsuc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xacnctag.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2azjutfve.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jlbwipis.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbcdmaqx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wqufuvmp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fbitqfqg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hodfmpvz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kmqqqstc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tbkrdzbr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vrabukol.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtzxblfv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cfocrcmw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eadhylwo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uvdabzjx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wwyfcduu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2klcptbae.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vdpcgkgz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2aluqfcnl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yxnwqtce.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mrbrdmrj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2resaidzd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmzdopl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vphnkvri.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rkdevkgp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kwqkglmr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zfgqufua.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pyglfwxq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qiieatfs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dlrapfvh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2cfussunj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mghsjbrr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2grnzinrw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pkhpduah.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2koqxgtao.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zoihvtia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pymngaag.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2myxomqlc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iytipgmj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjdjfgmf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gfhzjick.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2boylqpet.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckkhfxgg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2eufvjrxn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2swkkxqrd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wfujosfd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2endsjjlh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2btuvawcg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fkkiabxm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xshykhuc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2sdeqicku.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iultxxur.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rweblxyz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2twfhyfpq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izfhafdt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2imnowjnk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fpmywodu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2schqxpjs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cvlytotf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mxvkvjih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2plgagfcg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2unfxnexh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uvixxizq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uflfjptj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yldfeygu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qupyllev.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hedeogdp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zpdjmqxb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nzctjdkv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pixlbaum.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fapqeutd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkmdijlr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gyrnnurb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yneckhtx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qephjqmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwxyvn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcbyxppu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bsxbsffu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bruiebih.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vsiuhyho.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2evstjeat.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pmqfslyp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mmmwccys.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcsufhrg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2giwclzsp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2chjuuicd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ruzkfrds.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2slkekrer.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cggjzhvb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwxmstax.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xtqfpioe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ofbvnqte.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kivqauoc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2szvnadjr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wjmrqedq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zcacxcke.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2khwfenaj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ofacqolw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2shwjgiip.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mfzpnwju.html


<!-- 参考信息 -->