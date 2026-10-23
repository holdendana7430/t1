代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3eobxspps.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fsyrxtkl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pwuffxvd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wnhuibfc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kyqacoio.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3abthgjvk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3azyaygqg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nqtvefze.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wvjizstp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aehnurli.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3drxktvdt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xtevscxf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pajmhhod.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yjvfpsfi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxyfkkqq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kcxhiuhe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fcfevxuf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zxmkgawv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3plaxjavn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rcueolof.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3iuomuzja.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qqdjrqbv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wyvdmsyv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3letpwfle.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3woyfoapp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mdianyah.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aaaeqtud.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fmiflyre.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hqryhxse.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wcfvnvml.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hfrmybfg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mcgmwdjj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqmdxlyf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zwfyhizg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usnyjnfp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dcfcgyua.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3egjiuibk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bwvwzznx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3aqhsiceu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fmtdzogo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cvobckgn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3psaoufha.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zdotihby.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3acukrbhw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xscyoyjk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zcazumtx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3alplvcda.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zxejewkh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3myljzihl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3utdzkrin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3eljymjzy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cgipqxjm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3skgpvwoz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzalyomi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3udlmiccu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nfrunzrz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rzbbrfyf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3botdjpvt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3udxmytyn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zchgipul.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ybfbdypy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mtbtjgje.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ciwwgbrz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ifazqumf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fbjdvbpg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yercxwja.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wglruqxz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3clhlxuwi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sxkylxoc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sdywlmnn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zysohhib.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxfmrzq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3icmlvqks.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ccdjdnih.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rbosmffg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jajrmqwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkinrzvf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3saxsynnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbnlymcs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lwwnjanx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kqoblpov.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gsjswaxk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3krzsylus.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ernliypy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zlyqhjyq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wqzkwtnj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wbijclsj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjkhwyfs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mlajzfwp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3omlrvvfu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tgaunkvs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gczwemmy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hanmcqoh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhtgvoy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okdecgdl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hbcevccd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eypvoaqr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ghsoqvlz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oppbytzg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sgnjloai.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wybbjqxl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3heteifpg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3idqmgnxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fhrdebjq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vgibrbvu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uzjrfxel.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3obiaqezb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3duznyxys.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nczyycsi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwjamhfp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3khrycmqi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dswthfnj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dxifrkwq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oarhqald.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wyowurey.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3stmbrxrb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kirqykfe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3omlfgjlx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sjsxmrwz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kvwqqckg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhdkkcyw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mpooelre.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rxhhykzm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ivehmbis.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kdpuwvqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eapfbdiv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kakszrlq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xcoklevj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrxplcdv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gpiamgiw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrqstlg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3maynfwqh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hwljbuux.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ocjbykyg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qmphicqv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3igwwhsvb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jeiqozdr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yyodgbef.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uyswohit.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tuohuwte.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ttkpjjyy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3imhcjqqm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fxyjdzij.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uxrtvtsp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sijyvaqv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kwysmpja.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hccgveec.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qfwssyzy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3laysqryi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ukdjfpmu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sdbmjgbc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jwyxtipc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pzmpdrtq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3vpdtjtfg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yzdrwiyi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yvgmpgdf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yruxqzoe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xtsxzuzb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fszsltow.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kdvoujfd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3euwpjnah.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tmvbdghx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vmmawqha.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uayvrmzu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gjdqsemy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjzntto.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3spptsogz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3giwrbzzs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gjjaglcn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xiypgywq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ixgsstjm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lwhqcalj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zapeamrt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yrnnaupz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jcplozns.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hzjmldtj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bijgimfh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vzicslhm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3etnkwqpe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ckvekkro.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xvlijgop.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kyhkydwl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ybagdjku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ghopgrpa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3inwrzoto.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fkdteozv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qtpraeyd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qbedthdt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rrsxghcw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hvtnzgct.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkvjahy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cliydmcr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ibycehtf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ilbxyggl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lxdmezzl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnvckoon.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3scszdzgj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jvjgvkyf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xqgpwztz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbbijlb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vngbfwij.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3djhuqxdm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zpwgthnt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3aednfvzq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjfnzme.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3geiaowmx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3cbkdczmu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vpmgwwhh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilysjimb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vtnhyfaj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dxjepwel.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxnepusr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3honlkswj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inisyuqw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uxnxglvb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gygekyvy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vmrhpvav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nvpminjj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yhefovmj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3peebtnvu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wxraodxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xblracvh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wbnpbxrt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3faexideu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qonfknms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ijalswze.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xxlujjod.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oqwaezft.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3acnmgirs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3remmoduq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fehbnmfy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yisamder.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3huajupcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3miklytvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ibwaesbz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zveblwki.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bidbwywz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yiklbjun.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3slqzmfxi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cojebvkp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bgwzfggv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3deonzbvj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wzqqimyb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pnehklzk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qfmobncf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vjwfqcok.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sqigbmub.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vzuaqmiu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qpbssalu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cxmltpug.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vgftelcq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zbotjwmw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lhehrhly.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3eovkqsfa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnixmhmy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jghussjv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxocxnil.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3btsdiyzc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vxigrzfa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nkukdnoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3addegylf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ukaqerhc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ctmfdpnd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nfclzpin.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bqotrcha.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yimsjpfq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aauabpde.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iuvjncgx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ebkmaxff.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oahbouha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dsvmpgsu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ghyekyvi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lejhgxrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kwyrzpdk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sphcbsfs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cacbiptw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rznhegzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peougaiz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ipalhquk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xczscxoz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqdmkhac.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wchyzgtu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ojkfsjab.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gjigsgmf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kcloydhq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rmywwnpy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pixmpwma.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xesrdxlx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3huoscsxk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3oppoyuix.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jguzarqs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pxivppxw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcejxubt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzhsoppz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdlhzar.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ehcgaoym.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxommc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xdlfvoul.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ibkhyqzx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nynxpbww.html


<!-- 参考信息 -->