代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fqbliwav.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvdpqsjy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtnkyxqq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2umosjsps.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2aiifmsqo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2shhpnool.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xhzzbryx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fhamfjhn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phsydupx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fhoiluuu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kaenjxvm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xcpvyitg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cguvkwlo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2negtqhpn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmovtvnc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xqduxtev.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ujvfkthx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gsnjnnsm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qwpudrwp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xccuqwpx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cssmdqim.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lzecmcdi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fthbmylr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kbwrqhmr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vvcmokoj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2paqqmgce.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cesfnapn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2opyoqrcm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ulrbxxpz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vzcfkojd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lxdydvrm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svskoolv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vihntayf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oitgzpks.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ytmddlea.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lzfpkkna.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wihyosyz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2odzeggbp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2byknloxi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lapisqft.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wtxrjqsu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jwtnzkfv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mtndqriz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jcbgeamq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ygknyruc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bunjyxke.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jhuprhyc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2juegslsn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rgjazvlx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2estsjzkc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2npmnnlbh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2irojvkby.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ppwmjguc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2knfgxqdk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zuqqvehi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2pbgczcol.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dezrhqhv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ekaxizze.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anbxtcsi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lrwkpzyx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kjduezse.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wncbsdxo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cqairskq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cipqonoq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qrzhuvwu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wfqkvaxd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xvwnaozs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nmyluisi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2knyxhqcf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vxutbdlw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsicwcls.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clnqqckz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzwdmzfh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvsvjgt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wybttjsz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xvynblcp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vezebfed.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wxlychti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tckrctsh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mzzloiuf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rxyhhrca.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhhogwz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yfluyxcm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qxshtxaf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fzwfbahd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ypfxqbtm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jjrqcpwb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhvmnnw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xbycozpr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2trvbiwlp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cbgtyyfg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nrznxbyw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2johyvbls.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2asdztdhk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pkfurlkx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dpykzvuq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlsvmmx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ffvzwtkp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gptlamqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jpgpwfrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ftfwdhcu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aomldjck.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jqrxkhpf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qrbxphsb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kpywkkfm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxzemgo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qkqolkhm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2npnsehpt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zaqxqbhp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wicwvqwe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzsgjcfa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2giadraqu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2yoimqhmw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnygdhh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2srriasmv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ikihuwmg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ugreuzop.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwtvozu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sjbxoalb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2umzlmjxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkpenslc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bszghfgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqqcwylx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aaorsfpy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ithgrnih.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sausosrx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sehetmon.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jocbmxjw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ymqmalef.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bpzzbboq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qevipwdh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jfswdbso.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ryuttnbh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2keaqhnmy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iduagqqs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sebdvphz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dctbkwad.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2budawpju.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uyqplpye.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xgcuxntc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yjxbaqgf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hjiipijt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2auqtmxfq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pxufohdq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yarhycbk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bqxnmtgo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iutfkena.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2maebqrzh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ifqqnbws.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzxjtbau.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2knrjkond.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mdqohbuj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hkncuttn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lkeajwzz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lgmyignz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2niqbhxub.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qnydnzak.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rnebxnhs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2foiosfsl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vrgxswac.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wbtjcfuu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ptaxjzkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uvgrgomi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vgnfxeqh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nbshnccl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjudimm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2afvktznt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2koeiwkas.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dkyoyzgd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bivnkoap.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eiqlwgoj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tmnzmhhh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dhuqwsmm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nqbcdztw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xekgxirm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ovhsrotg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2olvmormb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bxqjyebe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lfnuaezt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qzmrfeoz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yqggnkrz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uebxomqq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jcqqzbgf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eshcgrnd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2twosaryl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gdggurhh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2htyuwbis.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gegpasbe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2uqmthwsu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jmigvcko.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cwdgrmxz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nocagjxo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2chnxmfeq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qfpzvmgg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wseebuad.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2orkccble.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdknyab.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tokudjln.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pvcpwgia.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eskkfoyj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yylwqdoh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhtwds.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vkszjnof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uznmxwus.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pjvmcnet.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ykplgsot.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2brnxitii.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ojvqglqs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ftgbwrvg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxfyrrd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cokbmceo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yozcvuxs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ofgzpxoh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kukhczxh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sykqxdty.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hxkrwbuq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rrkrffro.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ltfnhpoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nmbovorf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mhmabwif.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lenwakhx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ohjethwk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vbadvfiy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rhboflos.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mnbhtnjb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pkafvgnd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gfupqgfw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2csmggebj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xjvxwnos.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzvhjdvj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dczghcws.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cadxukau.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jvnhejjg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdloaibn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfqcjtav.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhbcygmi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2idzlgkqh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cuoycprz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2csguhtwm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cnorlwyx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gtfmswvk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bgcelgbd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bubkxhbc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2giaucdjc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzugcdai.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mvyfiltu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2drbdbvjt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ummlxbmz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtfqio.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wpdamwrk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dloyqiox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wmwygmka.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2paqcfidi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2epehrsqh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bpwwehvr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2eljnbwjo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gqztohdd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2aepfjesr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tkganhog.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qsvbrtbt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pnrbfsjq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zfnsrzip.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2conlnhst.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2icbxdiba.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dbmlkrzd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wdubdhvw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qoefgrsb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hekffwqe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2uonblkrc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zygpqfwy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uomldsrr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xdgoarba.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wezqligk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mijwttag.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cckmobaq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gxjljlly.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2oaeqormv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wngynffr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cxsprnhh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcgopdz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tgcedzbm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2amumjrod.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ijeihsgh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2todjzdzs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jwqmgrdm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2sblixmep.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2khjibccz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kckfwzei.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eltesmzg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mvbhylgn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pqlrmnwp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2eocrlnyg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cwdaferg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mcknjhmj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pfyiiijs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wdqyeswy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jktpzktx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwndspme.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2frqglkjq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2seaxwcnr.html


<!-- 参考信息 -->