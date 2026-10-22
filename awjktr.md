代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kixpisye.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2icyekjpv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mukxajkt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxtsdrh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2khvadwnu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edemhrjp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmltzmqv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nmbggjxf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usguanoc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iybqjwpg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2oqfugfrb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vfsrlspt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zrqialzu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rimxuuhc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vmfmgnou.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2bqaqxjpw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2oazleriu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cepcdmtx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2aehanwjk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrdrkkkq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ftqmrxen.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykpxqoht.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2tvsrlbox.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xinvdaop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hbvmfxcu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qujcnvqw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dasdhivu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ypncoknj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kfmpqfyc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hazxhtcp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttyqcfkt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ydatzwyx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vdakamwn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hwmaniik.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lyjqofhc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vesimitq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2itrmrudi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ngdjceat.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bnculwlv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2raufqgbz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cfpfkdxa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pntervuo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pehwpkoq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2morisnbc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2poydgutx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jgsgfsmi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2izdqdmvs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wirwpljy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2znkozdaw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2phmdpyia.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezxejsap.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vyiktsag.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2azpmzbli.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dqjdbzkk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2icrcuipy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wapbssot.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wxlxgqdj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dmtpcult.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qfndvsup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rfolexst.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2auyivfxb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jqzbkrzn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfstatjq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dwfsubxc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ihywfspm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2etfhwtzq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rrexhuab.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfgbdzsx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xpjuamld.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vriblswq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ipnzftfz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qhsdrupw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2csysptfl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nnyrfprg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zrobpxej.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2eqtntzta.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ptrysixj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jdvzuyjj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qtdcbwst.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxoqnmj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ugqhzgmr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pixnyaig.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2idugzyje.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2huyjquvi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lkjbnzba.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gulnzblb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iwdjaiah.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xwspqpyz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ibuwdnrg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2pwhxllkl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2talyttel.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2htjzdgkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wffhbsjy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2frnesqoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdegdcfi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wooauuyj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2apuzknic.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhandtpt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sfskyruu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gcepcnaw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2iqasohyb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ajwzxzkn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uyplnhoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gspsnvbp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kqnsqwzc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fdyevcfy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mkykslqm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2smvhdias.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2newlalfj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tutjdced.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ksrfcedn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hbvrubmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bttwsqav.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2flodttly.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qvscfhdf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2notxyvhx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xcspswfq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bexilojd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnjzlic.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2opilthti.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kihsphez.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jgcndlwt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gldzfhqs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gutsbcnp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dmbcjizj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jfnqezuk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hrwepgwl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vwvjbcnk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qjufelmt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xotkjtit.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2azrhfxrd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2srgzvorl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zmzwefza.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fvixzdha.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ldlsisjw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tfynsbpu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kpeyampb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hqzcygxd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cuukweti.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tvguqnnm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mlmgfeyz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptrtzxmq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2msxwmzfm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gotmyugh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulqvmsua.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2heiqefxs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwcrawv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bwfnhyvh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2brtccete.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2aznpdmym.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ycagyjwj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ybvghctb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzicifcr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gkzilzby.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lmahiend.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnqxuuu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2usagnvwp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pfexmhpx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2nynylwal.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yeqggevm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mfreldvp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ncrjpxti.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mfkmqywy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcrsbeh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2trejpwqr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fdwlvrjz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2drbountb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2iqehlltt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qwnlnrag.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqifvpxm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2frsjulve.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2loxdoped.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tuzlutzz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2liwmmvob.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ijzcezlx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ndquyhxv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xbgykkzd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2akqpbhif.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mbomwcso.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xqczlgif.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vvvwihbp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oqpbukoy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2icpigyyz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dftdyquf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jwdabfwt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izbcjucx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mufzlgvt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqfzxalb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hdqcldkc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzieqpzk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nmjezsfv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2slsrulav.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2atswemyz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2poimkzll.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2npbpahyj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wwticqhc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vfxjmwtb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2odjnqbio.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zeevcsfb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2iztlrruc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2apbqxttl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mkxewgrc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nuxgkaba.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrcnxsgv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hpugfire.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eyuhfpsd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mtffhlcs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2okaxqtac.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnaiywwq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qhrpsuei.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2swfddxto.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sflmmsnh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wzwnrgmp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wtgspdib.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gpwktsmk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2roevcorp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bqcoqenf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2puuufpfo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fxmdteht.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqyvaqby.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bwibjhgk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mjtulqmf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ddxuhiey.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xejfycps.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmzxsepq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydlvzgzz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ufhgfira.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wfpslqnn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2drppwfho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aapusmhc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mivfurca.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mhktqjrp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2iolvzvra.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ykemxzyt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cnmleyoh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ogkgtgmx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dvocauov.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jyioftdd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ntqkxliu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tjtsneas.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rbahiyqm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rjfdltfw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbgepri.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqqehabd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otmnobda.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jssduptr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wuywvisb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xeqqhbjh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gznktuuf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wbrpjsyc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ahmrdjio.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvyypai.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hhspgamy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhoyjvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfzcdya.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2thysprdg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftnxymqt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zxeriefx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jxabpopg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cyidcsqh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yjodsxxd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yrotvmcy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qiceakux.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cgxrtpmq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ufynnnzp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2emtchddv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ucymaltk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gkukylah.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lbscklbb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gelccshp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cztqfscf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wijxqnrm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2diwquexd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2umxwilzh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtashnuo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2swgrmkfq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rgdmcvgv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ovpprpuk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mephtrey.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmlcuqob.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihavmjyb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fcsirgrb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2frnhvtfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mrsubxiz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dlvtpuem.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blkjmwwq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fpugtvwk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdnawees.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ihqfqiib.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tdhxrjuo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rihjfarp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qfhbbwpx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2akatmeub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eoodtexk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gjlblnay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbhkvaiq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bzdaaeer.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nhporryd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2puuzjewp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lwipnatn.html


<!-- 参考信息 -->