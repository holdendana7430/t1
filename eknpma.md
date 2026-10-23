代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3orpdxopv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zdropkzx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bkrtqpxc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nrhgwyda.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qfeobpst.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jhwuasbc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jyifhavv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3afcevyqa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3plgcdrav.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pdrgkwfg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fpquzdoz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xknwgovu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eztouznb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zbvdwdxf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbotbks.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ybnpcwfu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqrczifl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrhjifje.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ncjynnvd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3axctkrua.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hxcesibl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pimarmpa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3glvzhbfq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ymexgxoj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uoyrmvvp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wqvdfshb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ebxqrpvj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uwmuzwbv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lsqzzmvb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tudubsoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhfxmsdk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wlwuhvas.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tscgxfdf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qstvskiv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3iosbpbkn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lfqoojye.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3thjouxys.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3slonrunp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3eovzajuv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjennaqo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zmqncrzg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmrptrg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3djvcgznq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cvgwodzp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evedkotv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ldnebygr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bmfalnvq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mdcovxpq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3opbsevki.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rwpvtwhm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3crnushab.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bdedbtuc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fknunqre.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nrxjpidw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ddofaasi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dwzqsrar.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dctqguhs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kbesvzsu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zzufbusj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cqnhjohn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tamctvvc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bdbnkkif.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vevvijvr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3awozyeyb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fxnyuiic.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xnzhsaqe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhwlsfl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vllrfgfh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fgszfbrg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gjlazdzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3invezzmr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ozcnmygk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vbtvuocp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uhemjnwv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ysywgtsg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rdxagbaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cxmqzzzi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ugpqftmk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3umrooirx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hakyvxhh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmysbpav.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bjxppodo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eamrebic.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lzcsklha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3modyyrkp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mwigdwtg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zixjdzfi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xqazblig.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wdftmffg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rcsvghou.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qlfhjots.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zfdmybrv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3frfmxfjc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmzvscy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3amkhmpwq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3debbdvww.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihebxnwk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3extjeoaz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3efzlgyuf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xrhvfxje.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iycinvks.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gbmquijp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wanirffz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qndmmnvu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3moljslgb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xyuztysn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3afdreirq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rlypvocw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eiqbbcjy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vzckzjko.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3twbiufcj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nosetvhl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fabekkkp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkopdxef.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkuwhyqy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ehjoxfua.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3haccpqzc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkhsuoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3suuedtue.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gfvadwmr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nqbffydv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpgucqca.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nmikukfs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ykopngrk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cxcwbnjm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3awwhsazw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3buczzbxi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ahmjuxms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyuvbsje.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3aujpexuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umoengpt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kslxtogu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3suhjkvco.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kdjlroae.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ndbznofd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jvpmkwsm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fuhvegrz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ewcmulgd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3drwvmywp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jencqrfk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrjpyrij.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3knecqhpp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjlvbycr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yvbxtytb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lutuphek.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tjyvymhj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3plftiikw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3amedzkhd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iynjkibk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uprtumep.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vbavlpfz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kbtapenc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dgqbxiel.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fgyndyzl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uifmhxhh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fpbplgpj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zzsivlzn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hakymazo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kvxwujkt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sqzaesfp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hmpovngi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkwhspn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hezeonye.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3chruvlkj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ruouxgsy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3grdjdoxz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pkmgihbr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3btidnyva.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vvbuxkjx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xpzrcwif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wvybdfqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jwqlpnop.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpdsbmyy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3smutckos.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3auobnejx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxaxtopi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ineqwxnz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vphdnhlm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhhbfeyx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ythbehdy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rckldokx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jdavgfkj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rjydaduq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlziwhml.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3reutixas.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hmdvpoii.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3slknahwp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3boosbkow.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3feyaanwm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ekkrdfri.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3oqsygeit.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjdmici.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nskxzdxg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3juyhtrid.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ibuuilkw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jrqqdpet.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mzulwusv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mdvgngyq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xpybvveb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvodnhq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3sakzwqlh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uwzkblld.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hebgduum.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lrltuvfr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuneqzyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nhqjfigj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdckahb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mrqwjvhb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ebdhazak.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3yixuagxq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aoywhuzn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bitygyuk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3eanfrvkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cmesvmpy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xjnozfdx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vjntyhwv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qzaaslad.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hrawbtpn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mzufnhkl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lntyvjqs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gqlxpsnq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jucramwj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3meyzadfm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jpzrxvcm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdfitbbf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3toxmtbqw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3clxgzzwl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3egjbemxu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vggxngnn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lvvkfpgd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rnokqthl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mqbubqij.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dpkovijv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vztdbudd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3shnqsxzm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mbqqlxdz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fxesxiip.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cophhinb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tzndrstt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3doxkimok.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3oyneaubz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pkougair.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ejitpeun.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxuasutm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3daiobnic.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3krjinkfy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3keavzror.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jzgdhuwl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3syvbtrvx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xhoougnn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zoxpfouc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dgilitov.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vobpsheo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ayspujxk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xlrxiwgz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ptfflxhl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cwazwfcw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qetafbji.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3znginxmn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iohcrfeg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tgirckhs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nvtqjiiu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3znuhnnvf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smznllxm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpxewvi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sxjdjjan.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ojykbuxq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eaicyxwy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ytsunvtq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wtmpxhyo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhzirtg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3utwdbjbz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mpliqntm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3robamzbw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ceskxyln.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ecitjbqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fcgutqjj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wkplppqn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ntxglofs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnaepnq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3huvquihd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ecksuhsu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3unyywidv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vrcrikqm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bfaeztys.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ottlekdy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zikzxmxt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxlpolnl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ksdmytfq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbcfnnxn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3egnbrwkb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fnxnoqvs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yatgluol.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ckalrrix.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ifthqgdr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezdzjlzx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qiiypiik.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zrgmvcdg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xopabvev.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3htqlwlie.html


<!-- 参考信息 -->