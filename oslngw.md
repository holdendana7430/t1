代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sfhyvhis.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dtvkndzd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmgedvuu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nyylmqma.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2smrpdccv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xorqxjsm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qcllpkmw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2crcwjdtc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kytqrlcr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kdoauawb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rurudsow.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezbjnzun.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gtgsqbgw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ogzqqbkc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vizrbyux.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jzgovfxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nqnwobnz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2agiuumly.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qevsstld.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zssfmwna.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dteozqfo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfoledxg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2igzpqikl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wdalxbcr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odzozqbj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hfahdfla.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2iiljbigz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hwiuridc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fgpnygzr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yncgicuw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjhowvj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pjemeljy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ltgfpkoq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2izomtmpp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xeyhxnoi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dlakjiaz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2chymkrtq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ctertaby.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lbfrxogi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zcjnfeop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2effcelfe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xoexeqgp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mekvpivm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2goyidmrw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2btxfaqzq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yykjxnxs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdnbarw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jgewuzkz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2piwblzxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2njaoxhuk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pixvgriq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kavdickh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pjffbqrl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zrxcrkjd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ugkjilbk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jhmtkeuk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2eiuklndm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eymvyeoa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwfiuav.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwaicug.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2myhuhxef.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvnshcn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qmpepgrr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zwsjqvai.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xvdgpfpf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dgjfgcct.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kitemxou.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ymnqonck.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rculpprn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hlgttvya.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bdpbotuu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gyhelwht.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cmaxhnnc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfonhnxy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxaxgsdt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2plfundbx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mzaueuhm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdpbbbo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yzmvwvfv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ltepcjbs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzyxymp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ndmkzhoq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vegnihsw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mpjvpcoe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sxebdxme.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lafccrol.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fnvivyke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vpefsjtg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2igqfcull.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ncjiimhp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dpchmpmy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2iaboccfa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lzcgjyek.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jioesgkl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2sfvwbwxt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfdhhstq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2crghdcgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hdurnxfu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlaxmjcg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oeqshuvp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rupckzlj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2auswsktk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zbkdkgst.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gkrjbsrz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vmkmzsaf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tltulnfw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gkggitwu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iiyeuvsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmyehgxs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qdacdhts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvurvwtc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfvfnxvw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ncwihpjh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gdunukck.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hlcemlfv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ihlqvpkp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hiygtmxo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dcakiewd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wpdceebz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lcwdmjoi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kddzwrpr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eudbhvnx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mvbejsxf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kreaiqpb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kvedtrxw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hdhkfudv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xqcmeuxi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2axzauyml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2scuhzozg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qrkynzfz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2inmtiood.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gzucwbvd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mygtibkf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tzntxvon.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpcydgc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2svldzvcd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mirepstd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ltnuwcqo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2guojximg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fggaybac.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wwddvcnq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hewjxumq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vslrkxhd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ddptkeoe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nqczkooz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gxjfeblk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jdzwcesk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2iyiwjaze.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wysughtn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xbgjldrp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uttnlxiq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zziehxlw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qpvsufbb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrtcfzm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kmospkjv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vnnvynmf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2decjcazn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wcnxdemi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgtupzf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcziekzc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2soemmxsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ofptppyy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grkttcic.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rhgltzpn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqtldmjs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wanlbaap.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uzlfurzp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnqhfyxi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ebzdivzp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2iuoyahou.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nokfmtvu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jxcnanfu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xkqwaeer.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ajixpaqn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iboheqly.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2smqmtevj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2trygivti.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xopypxrc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2awcibvxq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tjazergz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nvsrcxvh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sjzyvvdx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uewpkcpj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qycschqq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rxahylib.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrzjyenh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yxyzpuyp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xzmvschx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cpzvdtfd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xfepxppc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vyxpbonp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2apttevub.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nbsxdsiq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cimsftje.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kvbbxjoj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eimidemt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dngputjx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2idhlfzkb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cpiceetb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mxffrcyk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cxgzxaaj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cyxugvms.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nqvbcsys.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2amgoezbn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbwmfefj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pqiqdxic.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uuqkqkyb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wbdonmsh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nefhxbpa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cziqfxkg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uixopkme.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eddxtxdb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xkwcutdp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2otfotbey.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkujxyrx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bvkjqwqr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ltqpfbci.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2obxafehf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qczlhrwo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2sldtonbh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2agfqrnpb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gazyccul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kvbhzito.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zydaewma.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nzkqckvg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ldzxruya.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tkvrrjth.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqzshpch.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tezcmltl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qhntdfeh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vppbhzwi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdpblqa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mkdgebtn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uqerloyu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hwqmpdby.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mploleby.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fiyehqmd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rcumceux.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmotpdpn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wacttsab.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xuodpsao.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2emelucyo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2obvwhlwq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbpnnif.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2egleqqaq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2piwxpqat.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fzxfejjw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxrtkqmy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tlthxtbs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dzewvlwa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ktxogxgv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lkghspaq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rvptwttm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nfhoxcwm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vbendbrq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ondomlma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yepqakwq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgmkzmbn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkjrhonx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dbiakzak.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dbwsuejd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sfgzukio.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gwdzpkaz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2eylsxyqm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2svmevqxf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2imryvhkc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xtgcbens.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2urvtftnr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pgxoqewa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ncjvzpmx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ovjdoyjj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yagwjqeg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ukytebag.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ygmgofiu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tncjmtgy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2akymcvwu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hhzcuizw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dbdcoddk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kniphodb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fcpzaioq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2psilzsuq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pcaesjkj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gzvinpvu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mfnvegvy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2iejjvwde.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ievaoxbl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dokkturx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgxnhjot.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xamdgukv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xnsetttz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xexexmbg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ymnfjvxc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ivmxrflt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2teiifbzg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zdktgoju.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gczatmov.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jiyvlrgp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dayqreby.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nscuralz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wyyjutap.html


<!-- 参考信息 -->