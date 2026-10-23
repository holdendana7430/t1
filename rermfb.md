代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ctnluakq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpaidom.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ztgkyhcl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rwgjiivc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kilenadr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emodjsjd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxjfnwku.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mwgngfkg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3twyiimxm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3exfmbzpa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qakfqsel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fltsrnqn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3broqpxir.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vncorvpw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ckvlujlq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zrbzfqpo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gwwfubbk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vlszjiey.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uyagbyfk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3irhsatfo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vetkznme.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3icrefkux.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dljodxbz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vmtfxtvg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gjzxcyba.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3blksjgmr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jpqonyks.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3horytkhe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pefscvbi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3duelkrbn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bdhuqpoz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbcfrfch.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pzwaabdd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pczxbuen.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymnahkhl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cnbvwlmi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eioufluw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lplsjawl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3avwuhkyc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qtxccnhy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3byllsivv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xhhzqyur.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dxjeembs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lhbsrtuk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvfwzecq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3goeaoueq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3etnjyghr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hjcvihmf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fjiozowr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ptlpyucx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pckrmmeb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uzqamkvc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pjzafubg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3usioenis.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3btiacdsy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3maotjnjl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vnuudpbo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xjgsknqc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vmbqoxsw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bezwcfio.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3opxrnjbd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3utghlwsc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wyfonwst.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ogddzjkr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zduohvlx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zpgulkrh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tfpcrqmx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3teajjjoo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bugghegj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mifwgdvd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3risotwpe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kinlnjtm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqycaxm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nhldrhco.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gknrfarv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wxuwddxn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgqsodj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fwhpxuqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgpjvbc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kaxsienz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ilksqpjy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfyutcb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wlvcrlfq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tnfsbuew.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3huaxjcea.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mtwlrdcy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dofpicam.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qnhckfgq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pdvesxyc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gvwyqjbg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsnjaags.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qwtmtiti.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvwqbgfs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kkabxvmp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wwppncpu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3unvxwuzn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxbvmxc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yfiquyez.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vffrubuw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3cyonoary.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ckciybdh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tyercqis.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ushuevld.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gmqvlgpj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3epdxystt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szflaftq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fibiqesf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3afmhzskf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jjipfubx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zjnzjlar.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgenttpt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uewzqcio.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tzolipot.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hfzwzfsx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzzvryr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hplhhelj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3awoxbcww.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ycsnocgk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rlalrwna.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vwxamyfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwzgtjbb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ceshmmmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdoenbcc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lmjwznmg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fmqnhmmg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ggsjlxus.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3olbrvjdw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vizcaani.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3grpicnet.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aktlbxzs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pctclbej.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fdfdddtu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qvqbabdm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pnszsaxc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqsjxzy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uecreaol.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3thrjqqzk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3smnmokkg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qnxpdjyd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qobrxpsi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dkvlqgeo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mxifkiqd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3taeiwfzs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pnrdhzhq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zfhoriac.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3abqnoeug.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rcfaoaua.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pfuntpeb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xbkttygl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zdbgtuse.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pclvrfom.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3quvocerb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zztfrzpj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hlesfbsk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pfdeflhn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zvfduppy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hwizvouc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3imkanlic.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mucnssfi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hpihcvaw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dauukgjv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ygepvliq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qoezfsmr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ivoigmbf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fhtunipq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cukbkwqn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lxtxwkqt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dsqlchsl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3crwzmkqz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyqzmdsf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3paeqqbyx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkurevts.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lunqhqpc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3caxrlaoh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3evmeonii.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdtnxkbd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwbglkl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3okicndvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jojjjbcg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcxucfgd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xpvxhywz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ivoigffa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3iplbcpoi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auzcebqc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3znxybjof.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3uyahuzcv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3deudejoo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yqnthvbm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3osgcmhkh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdgtueo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iyibomcd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mcpgonnv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dvgudurx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zrssiack.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wvvnaugz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fivyxyuj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqhxqdq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngznwfsq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gpwczfkd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kfyctjhe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pbwqimlx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jyxeerqx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3shoytvfv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yhyktngc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3stpqfgif.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3srpqrexf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vdurcjas.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3igumtgsx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tepkrizq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ooiqvsmu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ysejgxtp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lolzkams.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mglbuxzu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ydqkjfxx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3msgddrjq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ruzhoswh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wcusyxnp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ocyygcvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gajnpfzu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nvwixxly.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hbpmyfmn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nbiccuky.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vfqgldom.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bgwqjdix.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dsqcygkg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncxszhzl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oahjedby.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hivvzanx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3npheujpn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vwmnkkbz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3yixiebea.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3amexhkyg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gtflrlag.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3coxvuocq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kovglamk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pczdnzyl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uzbihcza.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lihalhin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3htfbmhqu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgmecdgz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tjrrmnif.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mpouxsux.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qihuzivc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jnpivkyy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lktwhwiz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mhcxnyfx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kccnsskc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zemojnyl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eyttkrkj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xaoggloq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zcgzhvxq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nknjgsaj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vtxmftfp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3crzjijpb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lnpvqouy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdoncjqi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plfqauga.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uipbqhao.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tzbrfgwl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3edwdmbhh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wkbutfat.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qjqdomqh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cluqwqjk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3redvnosm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3blmwvosi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rnptnlmy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jgntseeq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oaacvaiq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3irjzwquy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hcvububl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjczfaul.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xhmoqmlm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfpcvquj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jejymdjt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bqwodlwi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fxfvunbq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mnlbioof.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3canqofec.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mcnevhwx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oisutban.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jgcmjlae.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3egknibub.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ijqlxrut.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wxlsfjew.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gktsqvyj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cdnyktua.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fofadmnn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ttndyvjb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gmzzwodo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hfeceafa.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tpqsplvd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fjhnhrpr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ojrvdlcj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zrucdngl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gxqpwnti.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wsboxvyk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ensdeibn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qsxrcuyr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixpouyyd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wmntdmur.html


<!-- 参考信息 -->