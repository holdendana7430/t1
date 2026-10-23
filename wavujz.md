代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nbrjcypr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3olfowutp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jkfmderf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bpqpraln.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3euqnoxif.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mceretwk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3axxnkxcg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gkljpual.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3njjxriap.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3riuttixw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkpvloji.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kqfxrdrz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tikhglke.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xomctzef.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vbdrnfot.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wvumwyor.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zovqujho.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mdrgncsm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dedtfgtt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3okzdctfv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ynabjenm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stasgjbe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wrkeaepq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hsgsgivh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjbmygez.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3npnczbsy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3swnlenel.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lvewkvmu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3umsfciwv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gxwjgggb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmiqvlb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3psujrdrs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xlumzcvk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tnybujan.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uajwusni.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3arnxyeyp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yueosijo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3alknhyyu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ktebxbvp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3txaietsv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kqviiwsl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pyswtcse.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3mznwsfti.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3chcxmuwq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pysgyprw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sppxcyym.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdyikcfe.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvsnhjvg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hyegaqoq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jkhakuah.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gbfdbdpw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xwgucnxn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3eivrngna.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wzlgkkzr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3eanralli.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ulknrqzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bopnhsik.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzeflehv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3beiebmls.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rugdewpe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3icievdrl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vaalgniw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qccowcpl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dmcigzlw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pfurwhcq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xuorksro.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpirkbuz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mlobcfew.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pljjwqto.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gfggoaeh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rezwxdzj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dnmpyqiw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sgkladvj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kbgfhgtn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wwooctlb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ehzoyeyb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgauwdy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vyzysvpj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cmgccogh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3atrjfbat.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3duflltdu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jzxudavy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pdelylvk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lkhkqumb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgjheags.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xjlcumax.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rbjhmohv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3madefrzl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gbnzkeoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3swutoojy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3udhbpetk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yfegbgaq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ouqcjeql.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aodeyhcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lelqraup.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oiycwmwq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mbzcelfj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hochpwuc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tkobosbw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zcdudrav.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ncxwinav.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zcbsazei.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3popvmryc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dopkvsmw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nfmlrlyw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ragscyki.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fwvhrxle.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ylwzwntr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhvmcrsb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ovrzwbpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfjpveuy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mclstslu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pktouanh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3utyrndra.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fvynhctc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xozntczg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qugumfmx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lnggjtvp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cvffdbxf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kfbzegoe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kbxpcosv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3htympona.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fnatfibb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojllpliw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3awsnqlnr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zitouxzt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sixlsrdg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tqemiury.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3flwwuegb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nufrjbxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3phpgesgr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fyovzfug.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hwycopba.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3luifchui.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cfutwmqi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tmtahetk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3movgwkdu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3brufathz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fhwgseib.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bdnqscuy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vfjvspxi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xynbotid.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3osbnhmdz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rclofvfu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rumwxylo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hgidddiz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wbsvgeav.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3duyeflvj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bcuyluuc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kruqtxee.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3trcpesws.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xnxvvssa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jihezgiy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vuwzqztl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fwimofcb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bsnxgzij.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ofzpqdjp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zruddqdv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gowxwclc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqmffoqn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qsmhurih.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qnmsofki.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3grwlnszv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dovyfyeb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zmpeuczt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tgthqute.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rqwgnoqu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfhalbxa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iwniwfdk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3babfctwb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ajbjcwqv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qksgwvwl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xcntvbvp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3queowkyl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3crjuwjbc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3obnhaius.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pcajmwmb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lgkipngf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lkzgqqyu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kwyzsutm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3oihuuzug.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3flmimnvp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nmubbiut.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pucbrzol.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fjxocgjd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3udbvxlav.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rctzdqkt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zjlzwmoe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mkgxdmvl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gmqlvlzp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lochmmno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qiynewkh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bepjonnl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jblmdmyp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pfsgcrew.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kxutgiza.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ciwcdwqv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dhuyjkjk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wvoayvnx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mtlsoiyu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ncnntuvy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pwiqyfkw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3snvxwnou.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yteicrjw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3redlvpzs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nhvpngjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pvgthpmy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rdkeejej.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nzyclanu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bmjmbyrk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pmordmyr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3czfgztpq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jxuppqos.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fiwhamoy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3malglced.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dennsdml.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3quaoouzi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sfevigqg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sfnociaz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3iydicbdg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwxymxv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qepkwwhc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkutzzzr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwqhsuct.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wosnxtuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3eyhuoyex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ayormthz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfouegom.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kixwpbjh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fzvswzqg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvljxuzs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmaoifr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gdejmmoa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eltywsys.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xtjhbpit.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bawrqotf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvockwm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mhqerywv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qwdsunkd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dbzrmndq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxavcgxy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mpxnaitm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wxgghmrs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jsrlxklv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcyplntk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rpbmyagr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wzeexdeb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3meaneble.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3eyjmduty.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ptlccqxr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xnxfdthz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dxrtsroq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcwtxuqz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qrcsqppq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dwfnzano.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cmnjbjzu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mcilcxre.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3inwnbmgr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ajihalhl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asazhilj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kkkoygwv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hhdojeiz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zobbwqne.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vxlvcgmv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pauiuagu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xgzzwanx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3yabhcrrf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gpzxseqr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fcrcewpp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtowdjd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsdfquph.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qhxuwrxh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcgecekf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xyfwnspy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uaktckey.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmcizzp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lgpfnwms.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qtpudrxj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxdzedkq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fsqfhnrq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3llzbiicc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dxkmnbcq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3htoctnvi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yzcyxlbo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vegwopwz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eycfvdpc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gavhtphy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veujmjqf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbhjfeyv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vexelpie.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wjoothdn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ldqkcoxb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ankdpgqm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3silkucjb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3icucfcrz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vejcgehb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tawweken.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jwxxuthc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3azwkjlac.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xqxowjis.html


<!-- 参考信息 -->