代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pcohpclh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fkjhnwpy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bybfakia.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3prsfbhlm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3naqmsmsl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lohsborg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhajoimb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdorsfjg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3znqwmcxn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oexaseby.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fcrhxpcg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vhcvlhiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3czahahyr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zwwjbzlr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3evjogdim.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwyfljcl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3klvxwjdr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgdeqva.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xqfvzazx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iqxirrdg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvaabqee.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nsnlstxq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ljoiltuv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wssbluig.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kqbvnqio.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3alwamjin.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fcsgctug.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cfeztjpe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3shqrnxga.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yyascnjk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pceykqsc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ghoyehro.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3efoxlmph.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wddtouod.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3oosowzfo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vmvldoit.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3svlsgovj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3efrtwgnn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qhgfpnxe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uyvpnsvq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3casxbkgp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ooakgory.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlhhknn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yyatjbvf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fcqejavl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yldhmkye.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3iyscvaze.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pllpyqyh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xzjaeybv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jbzxortq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3krvcdxts.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tibuxepp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vgmetyyi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oxwvebgr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ristrhma.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3prqptoaz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3haquvnim.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qafwgsvq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uizhceln.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3drqkxgzn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iazhbwhn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wkgzqfqf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hodxtari.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sbzeqguw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dkjumltm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3sfjmniqm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3teswfnfo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yblbqvuq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eztfekyq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aetetodg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cmsgnepb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pjjjvlzc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gpfmsbox.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zzfpnele.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cbwzlptc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cubwmqkt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuvqhxt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ygfuhqza.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iduhpipe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mltywxby.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbqtdtkc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3runlbnnw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kawdsify.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qlmuycsq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gqpolchv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xzparjdp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mnkihoxu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rpzwitoh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3afccxbhp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvyvlao.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pcyhzlrw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uhlgfmis.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3oagvamyc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vmhfqnbe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rifseriq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bturpnyn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kmqeicpi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibstwlva.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vgvdaqrz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tlcdgkpk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aiovncfe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cywdyqgh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zobcxtia.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zsoohamm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yikbcede.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3youwmdvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgqcatap.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3odncxyea.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cxzdgeju.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kuznidnk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ulrjxrrt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ddaycciy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uiuysflq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcbxbzse.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lbnqoqiv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ufgckjyt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kziasslx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xdqmwbdl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ukredrhs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ditibfdd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dapytdxa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuwoqci.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ytrcynkv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pzacccub.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ypwllcub.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dsljqukc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ngahlnqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ptedqyud.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3evmmbxyy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ohpyohqj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3guuszsls.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mkiuriro.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3voycgzqg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3atakwenn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hkzcitfq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pxwlwnge.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fzoosrma.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vyjhtpsk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlwycylv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dmxvjjjm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3imurxyfq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3trvqfmcv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cdmsvmrd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3eqlhvkjm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dfyxjayo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qezxzdqf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mibbdhjy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tmtiorux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fwczedwb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mupleolo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yuidthgp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wgozmhfg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zbqhbuze.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zkexwyzs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hdregigx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fkxffrxg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pzblmcaj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iinbaadj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nptlvtip.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vjlssixh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jncnsuel.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pkczbvjx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3efvkywxi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbcihlbd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fjlxdzrg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hvwtbukx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3syjmllnx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyllhqae.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yrscmwsu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eortecge.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rctvoxbv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yoiwwxab.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zjnduywl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kshvklbp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3etccciro.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jdmouglk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3iazybsmk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xuovvwqu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jlivubio.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3phbqdzvf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3blwhneiw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmrkknsi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mupeheur.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmrbyk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3czeanubl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cesxvxuz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mcwejlxh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3btzrdnwk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3odqsjzpg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wnzzjqtx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3egtgtuou.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sfyliulx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mhznymxw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fcmjorrr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xkhqiqya.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3krxjuipe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qlhylilr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uhmqdhdg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dcljphqu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3plscleau.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jvvfnegu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3loqyfxar.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ciojuzrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cgjrwiba.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lsbakzgw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uxibekha.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cerdocgg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bhlnjkpy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bmetumks.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3awqwtegz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cmhfnlgd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3buaxcjag.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3znminitr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3senepfda.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wjwljfnj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tklyjtuz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3aocgbzgs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vgeqttxi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sqhaldrf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wdecqgon.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bplhdeie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdkhxsww.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwjuqqo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqhxzfme.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qnvfjujn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vvfciggk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3avzxcoko.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zqqlqslh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpubyula.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hhftoxlw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zgouaumc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dvdkpowv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wtrdvbaz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ndusakqo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txpmntcx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rwvleoow.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nspewnyk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iefqzfof.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kfhugmrh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgrvpzyn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bbknseym.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3trwwyadk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bauopvkc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cgjydeur.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vtzknhgn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fpcxyxob.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vzbitkjc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgnyalw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3udskdrsw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mzopcpzn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nzpxisjd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3smmpixxe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3szlxwzoi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3amuujnch.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqeflnmr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lulticlu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nrbiwlqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3suompapd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zbtopizb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pklodykj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zpzllkes.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxhanoz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xdtwjibl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3izbzvbau.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3trvfpzok.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zcxjoazr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qgvhinea.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ngexmgdb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3adfpcoix.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fwndxdal.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mtolxani.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yohukkwr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kgfwcflw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xiizbasq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzkaybpk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vttmwsii.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fbmakhwa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hzfgmwtm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xjljlkqa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3asdpwxjs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3clwxupie.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3junddurp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3azhgkkvu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqwwerko.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdvrmndr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3otuxudne.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ofyvmwci.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tdeqbwxt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mangskqh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vcwcauih.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3opzsincr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pazeqgqv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ddwnxwnq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3idrwipqp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ouqjwpil.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oreavvqv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pjtipxvb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3griutbba.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wuhhbcnf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jsmijaei.html


<!-- 参考信息 -->