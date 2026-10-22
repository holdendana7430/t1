代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jxoeurfe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2keibwlae.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zaczftql.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wgaaesqe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ycffdpum.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhrrltao.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouslhuzc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amuqhnty.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lstypnhn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bogjvobm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yicmlbnz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jrgtrddk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hqyqheym.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qwcmtyja.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dwiifhjc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vbstcyxk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2esreutpb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ixxdfddc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jedrpnib.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ingocuvm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2urcgkjxz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2aulqpxdu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqwxtkhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nubqivvk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2owamyxng.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2htpnjsgl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dpbwfznf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dkxoxykv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uaqainud.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gibsvzbm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ldrledso.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlxqvkw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wiqohowe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iuixkbvx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nlxmigft.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2boabnkad.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzotvles.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kuxcskkw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mxinpcxx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zeuxbzez.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2goyjvsnm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ouujzpen.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rvufqhze.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2igicipvt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2obokxpqh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2crqxyknr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2aoclgyse.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckqvexph.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dweezoxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhrksey.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cosbikkp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2oovecego.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bnutvinj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yqlrssuu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2obnlrxto.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fgvkpirf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2adcbrrzy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ikdxkarx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xvpbgeeo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qwlyjpvb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jhvlioyj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qrluoeyq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fjzzmbxu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nrzvzedx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2asczulnn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zepkqjgv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2roawpmst.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lctzeswo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qofbjtmx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yokujlkv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gkeqalij.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aenojthc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzlkgffu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2twayhbqy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezxtcttt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rezejikp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ljmfmbmq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vizijtjx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2goagsixw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vlhfshqw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2eslkbfzg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gpwfhjeb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fymfmduq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yngtrlxy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ampsbntb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jnxdpmgw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cldrixvg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2runfxtfj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2utawcaii.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mosdqzru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2evpkyjun.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gafphpjt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyecfdgo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zgpkmckb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tjtroarn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jgjiibpx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wgzgmcsz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2skmnldzh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ivsbhtkh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2isiffken.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uwshvfil.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vewixjif.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2agrrblxo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qzvkpccn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tgtidoyq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2barrrssg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hfoewncs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtqtghg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ulpnjuoj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuldrpht.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jlneoiax.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wncddigj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zsaootmm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gnumhykx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uuhenmsg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hxsmfubs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zcwqjaoc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xmnplycz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dtfeqdjb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cipispky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujmcvjyg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sknvoggf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rworbcnc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sefykpnx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2txecaksb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dsfoismn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vtwbvvgk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oeqgztwd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zciwzhmq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2klykumza.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ntjfdspq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2idipwebd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gwdpycjt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vioegdyf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ajvneaqr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2klsahzlz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fujnqzpv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lvwjybfp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hqfptcud.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2alltmaxr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cxsnpxov.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2emksysnh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ethgoevh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xwwreumk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xokrwpir.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ebparquv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jxbwpozl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xceenxxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cqeoaynf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdvhfcfd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rmzcebwe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bxeywnir.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qrddchba.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2virsblbk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2frstmdbt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2icgzfzss.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vhirpbre.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uzukayyw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ndxgkksz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cffzhyym.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uhqggsgs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2phrhymty.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bjifpikh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mkcgiuwz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjpvcdwy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmocyin.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xkjopqhx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ldolitck.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yxwrncyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2moraajiw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibpcfaaw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frisyfra.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2blrruote.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbcntyrb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2thyhameu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hgghhtcd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nppnhglp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cwjbhplk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wmlvgikt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gjzplgrk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hkeurcud.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wsxjuyxq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2agmyjmnj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwygykq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mtsoindz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pkbllpbd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vtphsjra.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2iuofrwsf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xlgbkymy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2odqeirsv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qedabflx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmrqecy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2eyuzbbyh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oeoyvxjz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oyqfwrva.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2iifenvxa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cfmahjeg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tqfagaim.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zdbaealz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lqztbtdp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fxzdlpak.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lqkahrkl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ooheejln.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eosemtrz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sdrvvuup.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qxjutkvw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hjzqrnlo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2etmlukcz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfuogrxq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ljzbqqhe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2juhlpjgi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dhitgyta.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uahsknkf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vnvsdxyv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hsqhokgp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2keiikvgq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yhwnexct.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ruckaiqq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbyjqotl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2luvbzazq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nvojhtts.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bsftyzae.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qgjpjflf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kgywjvuk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rotyjymp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cbborexe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zatnhxmb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2piwlqjzx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rwsmbhvi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zvqoggys.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zckoxsnt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvrcllao.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtokuid.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kjjswcap.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qofcwyph.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsgavhj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmuimea.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rfawwkci.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2chqzekfp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rzqdvldw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2swhovzed.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nnepkvas.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fpftacuz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vltkwibo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsaecrrw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ukbmutxm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qpkmnfwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sqdjwpjz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gyarcnkl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2brjqrirr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zahffecw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pafxgwos.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2reymsoah.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rvtlcoit.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wqbrzeer.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2infsytyr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdugntku.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2undgejcs.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iefdwcck.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cndwjrax.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cwkrhlxt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jcpsoczz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mjlxrjkp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kzpycxuc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nssezlka.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2stfhcxrs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tiyitofk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bfwnucwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tjrlbkje.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qaoggpiz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2emehwxpo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bkathkqq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xychxfsi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dbewmybr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wnxsvuhi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nxschted.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kmroiosi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fyvbccko.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pebmrzlb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aviyulto.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rmyffkkt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fzrmyyer.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnafqtlr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2youtjnhd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ycbygkod.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2irisiejc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ezbufmdu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wizjxtkx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xcbtnmla.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qqukoszf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvsepmge.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2llgvfexa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rzmawghp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wxzoxphc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ydgvlvki.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ocpwpeso.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wqpifqvp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlwdegcb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jscvvszc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqduqyzi.html


<!-- 参考信息 -->