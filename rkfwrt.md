代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwtoqwkm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gutzdazl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqingyu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gxvekqkf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kfolncul.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3chwstbad.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhczontz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lklsccnw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jxufxvyg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hxstdwmc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tgedyryb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tityfrjr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dstychou.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3idzxkrsv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3imlzymlw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lyucikng.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cdrnyvuz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iebsgrki.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jgurczmk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vdpxxglo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tzlvplom.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jdlsttlk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ihbsnrag.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3entqousk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vtvtmqiz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlgkpggr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dygartsf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nftuwsdl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3brwbugrk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jjddxiue.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mvkhmpff.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pgmnrcfs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3sguslcql.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bjisxrqu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qankqekn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fpgemoeq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dgzxsqwk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sodcxdrm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kpscxqzm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lovgbmnd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uhiyttvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lesgmymr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3muvdxvdn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vwnnxvik.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gigyjwbk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mrtnyjoo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ejezcexh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rrqbskuo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cvlmaljm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ppyyxdbj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ljxhowug.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrxifbv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zbvjxeom.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3opwjkhsw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iyokfxzp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ihuxwvjr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zdfgwfur.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hzcaizup.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3onrwtnel.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cnhgxkww.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tcvmdfqk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ttuktbhc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shlxtykv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vkbjaxjg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ogfmimug.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lxjnedpa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3scgzsbxu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ogiorwzn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yettukku.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pamutmir.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqzcsnyz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gkkqffxb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qosugphg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ppnpxtlk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3cxppwhew.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3buryobpy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mzkeorhr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezvafkul.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ejlxbnwz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fxktmrbb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nlitesat.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xklcatqs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgityohk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gfsyuqhy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3snbreyck.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3woungcsv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yjtiwvwa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qhovxziy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlcsxhsp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ebszzlhv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ahidxqph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bblvqnmg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ryyjzsbp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ceyfgqop.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vvtovgmo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3onpmnfyp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mbomhhmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eacwtydv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tfakhblz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lapcyacw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3clypuohu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxvrksxk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adwvnnel.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pdecwyhi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nzgmlmfh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3txuaeuky.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hsnfibbw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aheswzvu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ohylzkfr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xrnvgszs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3anuoqyzk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwyxdat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpzrajjk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3izuhmaok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhkginwp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lfyedfbz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yemjljuv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3djfyxwpi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qqdraguy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bwgelhvx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xgrvfdhx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rffhplpg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fuxycuhh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ynoohcbu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jevtyvqt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ogwyemcr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qltbslce.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyzkkbji.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kanyaijd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3flaxerbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vzdkzhop.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zpdkqiml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sirgsofv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hwhhxzcm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3shqmwpki.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zemwyyqe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3noszosty.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyxygst.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3svkifhqf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3domvpdeo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jvrnglcd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mjithuas.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dqwlqbfq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3afvvuscc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xvmvgyzq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrugrmya.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbzkkwx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bcdkzeqk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qavmjnaz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xfkxnavo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qqmziyll.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xccnrwpr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xgrlglof.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vjfbpjep.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3szewcrju.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wyitocei.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3svcnlniz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nlsttqdq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ldvyriqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gyqbvhhb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vsktlrew.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tsdkdomr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yifqlspc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fqufgtax.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xlqgvbsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkddaxng.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iijxfyyw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xvdlpfxe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bkliuugi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lnftyqpt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rjwnwaek.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uyqindkk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3flaqtpqz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ykslptrx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kyoejmsy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cjcoeqqo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3bbfrpqzm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dbiuxujd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xbxuatqq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3luxbwogo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gofyqxpt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3esbjzpki.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hfkfmets.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pbgbzdjz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tyqthxos.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fkuyrqnq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rrsprtnu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wbqjvets.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhlxgqk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pjmydbux.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wfmtcbqe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtqcshae.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pxujgclq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yqrvwvaq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iconcdqh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mdqxtsdr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jrjzemqt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ktkmgfpe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3sayheprn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zdwnhvol.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3koepvmbc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bfeonuml.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gxlnvwcy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tppvugox.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rmwkmujy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kofhybxm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fkmhzqov.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3admdidea.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3otfgxcnn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bzhcsora.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bukhnogb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dpgnwhaf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yokouuie.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zqghcdld.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mptvqmgb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cnuvfpai.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eihgstfc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3blnfirja.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqykfdxj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3endhsbjy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ajbrzerc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3aevzkmrk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ccxatuln.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ojlvjxef.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3veneavyi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mypqktia.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkptrpdo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nmdxgnnd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oamqlhkt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xqnzslck.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zjdedrpe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmaokxuw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kpmatzqf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3syffmvjk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3knqrjchj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wgvpilnk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkayatu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oxjcmbmk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qekrxwfo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3skxfclsx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hrjxeulh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ditzdlsb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nibtynej.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3prlvesoy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pveahiau.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eptsitou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qfyisfdk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zurigmqj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbmmzkk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xjbpwoxd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qyxsxxoi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ghhwkyhl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jcecugqs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3blsstech.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3euqppwqs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hzoanbna.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tovwdhrh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mpsebtkx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lmtiwgjd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jkdvltie.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rebwutwn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lljpwfzq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3degokuai.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okyzcczz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxjzdiqw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zriajwrf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bezlgdji.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gjphbyhv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nweipaes.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3laoomkku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3vauuhiqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3usrifksu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aakyeijl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pxjcdvst.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cnhvkxnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xmaaxxtn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3orptijhg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3swyodlba.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3iqeffofy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ddaaalyy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vcwnkttz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qxzyqnys.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3koxykkjb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3stmhgnum.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wjbaasdf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3afmgeyzc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hidkyvqu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dpixncrx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zhfdprbf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xzmguxmx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vqyfpqmu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftflvoge.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcrkhaxz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fjtbrnqa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ztkmnsdn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3llffihuq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3awmraoxt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qvammkek.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vmtifetj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vwezgwsg.html


<!-- 参考信息 -->