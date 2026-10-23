代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3axkvotkg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ksgfdsoi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sckjjbhb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgdnfls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3itjaghpv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rwwkkbnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wrxmpsib.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oaiwddwu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kkzbrrpw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zzaabmcd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qsjrmvwb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eiflvrab.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dxmzwsrl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3spubhaha.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sejlgtuk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jusmwwqx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3puhqhdum.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fsebdrnk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3legncckd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnoqcond.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jnwshbrf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mbaznexm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3khnvhnkr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qjihennq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gorfuqbj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rfislbex.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ngisjuty.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjbqpdjw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzbkwitl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fkojzats.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fqcckbcr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mulnijhw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3abxssnem.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sqiwpbkw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3biahekyo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nzstwdwi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ktodtgtx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3blbidulx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3uiojndvg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zecrugvm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ixwxwgvh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zjsuqjbl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zziexhok.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3heegyhiz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pxrgagei.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cdfdnahe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uaccbrpm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3psuythff.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3imsavbti.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wyhayylg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cypozunt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fyjxgxhg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qfnphbdv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ierosgbe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugidikfz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dcymwhmn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dswscbhm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ehgenhgw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zrbvnjep.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dszjxzun.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rcdccmbx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wxzperma.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3cylflbry.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ksrlmeoc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ddazdabw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sqyxejuc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hioheyju.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wpgvbwae.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umnccmgt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qknmccdi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gcwprjzr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cwyondsb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gheedmdo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ygkstfch.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ypsryqid.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tsjgcamf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gzdqermj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oarzidxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3epvwzgnx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cxfmmlcc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nhdgrpqf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybeffbnz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrdsugzn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sohhrxeh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmghwih.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xfqbvhud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kxfkxtqm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xvmbpjud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3agiuylhy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yllsrqwm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rfsnzxir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3socoempg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3uhvtzhnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dmnacrdo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vbvnucwu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qoaouieo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qsjbdier.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3skhowlsn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zzspaegf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jousipns.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wimercer.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lnhsefne.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ncdmpmvq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdqluyu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3monvwoeq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iemmtwug.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mznvpean.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3nutomcon.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3alsxhwmb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vegwfxrm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oajgaezr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbsbgduv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3krrdlorf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xugtovyt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yyuqxsnd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cvnionws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnjgmchl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ipliafch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruxhofeh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3polbnehd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3onvrpnds.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pzisojry.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvzejxpl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vmytcaah.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nrpqwnqy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3orrveckm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wexzdrxj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oeimlefo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qhukvfwk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cwprapex.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vykkyawh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnytgflp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elhgmoct.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlfnfqo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3slmeqkdg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vinexppa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3urbovifr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mlsrpyhy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dticcdpp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wiwdepxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrjtgqf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xecapcvq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdwaszc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dumrjzib.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nhecnykz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qeaahnjp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3iefberzn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3odmvwgww.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fpnvlxqp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3itdjchyu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmouiazu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mnpgokix.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dwgxliux.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3natzujdg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpqrjhof.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lzhctjut.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xbsbrrwl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3biymlzbp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqmirmzy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mapkwumd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tbeyyhut.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qqwgfyeo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nptwrhyp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3czomezrn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mjmchedx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oghaoqmb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbqdyitt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ceerippp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kqeupnzf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xdiriefe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mbofwsgy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qybvzwci.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mbmyvuos.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3egmemzhi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hjhegxvj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddrupqey.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yojhwpas.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nlobwzmy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ixkzbvje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nggqkewt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3bjlpglxf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cybclysx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xdckgorz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lvjghvtq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zfgolhfz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kgkttulx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vmkhuytq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3acifqbop.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fltotffq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gkcigyei.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3grqdpzai.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3niugbooe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwfdbwi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kbmkhirv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fdjvbnfq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ypxohskk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yshygwvk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kblvbbtd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bsovlywj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kudzfzpb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qggudpdy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zofwfsfl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vetjmhxw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bsarhwrl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bsucvpzy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3enokhbjm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ahgksxzh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qwunlrqf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ozdtzuez.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avsjrctt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zyugdszg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohhwcsxf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zleqgxcf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ncyvoyne.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cashgcik.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3awounnjt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xzigvndb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yzlbipze.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mcdbhzgh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ydbuerbr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3evjlcwev.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhmuusbo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kttkgsur.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cfbcnscq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qcscedwl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tbfmbnnq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nijtxiqj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zzedjqgg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3isuepmwl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ocaecxqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieartfzc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rphullip.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ussujomh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yvxywqzs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3babjyidb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bjwlniiy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qfdpncuu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mwtumwiw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kjakjpgs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mpoksxbx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ranoogjw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmhkqdx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bfkougmf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hxmijlcp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pgbwgpcm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vvqbyfbg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ensjpuho.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ytnsbcfy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udcakvst.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqcbdhak.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3brjejtoq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbrmitwb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxnheoit.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zrlsepco.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vyluynho.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eweltvou.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cdritivr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mpmwsijw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lrqwwydt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3paaphgmy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3emhyvwgl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hlnnemqj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bvzqmxco.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pihlapee.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ryruaojd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bynpeeom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gluvutew.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytbunxns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3saxqkswe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oztnqvsa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ueimkfku.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vmdacduf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pongfdzb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwsqwjd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ixtkbcay.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eymvhgff.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bbkydyex.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lzpozirm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gasimial.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3iusrqbmp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cyugodvr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lztwpeqf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3emegvyed.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jroxqfme.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3trxvfxxk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ofligwkw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rukzfvgr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oepkztdw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gcccflzo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tvypkhxh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3syrhmaaj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tyjlopih.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ilnsxuyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpmkivce.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3msnybwzu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pfzsenpy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3crbadqht.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zfnoifab.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kltqcgij.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qqjfnoqw.html


<!-- 参考信息 -->