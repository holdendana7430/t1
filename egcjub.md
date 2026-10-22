代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2eeegovio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2licdoxho.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mzjugkqt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhnuedz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wrarstnc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fevkhnfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jwhwczhc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nivmxpad.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ugevvgde.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yecjembp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywvobqus.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tjqehowz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2drqifdwf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ohyaosxm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2emamsckf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yyllyuya.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tjvchong.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hszhkuou.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdpltwh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sbphbdnk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2assyrovj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jenucsul.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2psubzwhi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nhwhjpwn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aixixlxd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vsliwmsx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2waecdfmw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cbyeviom.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2biwkgfir.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgnnbmhd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ttshvvng.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ixikdxww.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvkkviqu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2seprwatk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zzdppybq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfalijrf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ymfwsogp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pyychesq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gtgplwjz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jjnqhqqk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2emfrrtqm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tjghkuts.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zxljshzw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ruvvsceg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2stcesazv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2otrqgmtr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ieaxphax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wobejole.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2klshfyru.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2femexrqh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hhigsppz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2aupbfpxn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zksmjysa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xprgcdfs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjwehoz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xplwfyyo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sixyynzb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmorirge.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nhfjzthu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2urgiiqpv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vbfodxrq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pirzdvcg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qwljewqv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xykenvdm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2utdhhxfz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2utpuhfyd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzjdqxd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjnfmikp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzseqgdn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvvcjwh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2heggzxlw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2pngvdrvc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xubmcahr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cvyltyso.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmzwncsk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qikspbij.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjehie.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yrfohpzw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jxzrfcno.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ythxjfud.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ifvvsbes.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mbpmmdwb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qateqjkb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jinzggmq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jqgclpzu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2aglxcpfd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ffxqtuek.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2aoieweut.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hyztmsda.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2detfzfhi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wrxaoqig.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2quzpyybc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2uyzysxiy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mcwtrnmw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fsifxivw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2lhtyetha.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rvaeyzzg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zimrtyzd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bvzjnyeo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bylzirkq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iitqylol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uiyyvhkh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hnrxpmix.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nfqgegyl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wggqiykd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gionnzwd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drbwbhfz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bvfgjdsx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fyuwvvnz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvomumyi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2syfmoteb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vhizeuzj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2srnpvfhb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2olrshnbi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xmwdydeb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qdcwjesi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezviavsi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zqgihoeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dihotqjv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mkltxinp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mnjelotk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qpfkrjod.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2goxkwepz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fcwhqobs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2iloabjaz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iyeairde.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xupmjrxv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2okccrsfi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bobhrtrm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ezizhydf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2htteuhng.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bquclhrq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jdpzinay.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rvnsncyd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2imusuptq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2svmsfrgf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xxosdklg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2njfdzxet.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qgsinzzh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ogxpvots.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hfzrmeqw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhduxlp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2krghdkwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yirstltb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ftkwoyrq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zhntyqdg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yuwdsmmw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wqsxoypl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hzarlttv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxloohp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2juxtrbnx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nzxuehof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2etpzubru.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iboaovet.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rwmgvoep.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mwgpgctd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hftljeey.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jmfhcizv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2srtuuqvh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gjeoesyw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kappvqvj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hnzirpao.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2moxgawxm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ppmaadnp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2twhafsou.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjitddhv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2khcstozb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ftxxfguu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dbcmtysz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tgxhknef.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lsaetedj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bolcjpoo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aobprqju.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pwltilfw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ldnstavk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxvodtmv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2guiqrhth.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dfbvjppb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rnkbdvvr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqghpme.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lyixafei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2naveemzg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fqjqxssk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gamjggib.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vjicgrco.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lfukqxxp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ibleqwgt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wnvnwibc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2envlsymp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dfxzkcvx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2twepbfww.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2udojtlmo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2akglgorl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2phaaepjj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jcvcwpwf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cqyuasrw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gppngocn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pxyvrrig.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yxvpigcc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wcqnybkt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hbhjuspv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dpjcsqas.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kisxsmls.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eabffjrx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ldbhcjae.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2twiwqjof.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gykjxsie.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kcrnyrie.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pvqjnakg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbrtgxpl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hreuysgj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqjhhqna.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tizwbrsh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rkaheklr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xoofazyn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tyxueate.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lmlyvepo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kdzycank.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qgsjgkns.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kcmebbxw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fmundvqm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsfltgxu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2amblyzqg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qtgttlyf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2chabkyvy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqacizc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lunaupdo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wxdjerua.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nkmbocdu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gzvfqktm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nawfkaau.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihoqynki.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ftvtskbo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2muubbuvz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mmmzabka.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwwuqsca.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zcubmrzk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rtwnxpai.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rrxrfdsr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2oshcpgch.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knjisivy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2epeuxmgj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jqutsboh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2almkekfo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dycvfswj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qlxpoecy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rghurejj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isnuhtqk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlwvxjsw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2elszokys.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2usrpthjr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qywvgtpe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmtfxph.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ontvfesv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ierehxps.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rircemtu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bratvsqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmpyxp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uqnslutb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2suopmwhv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2gkrmmmbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dfijsnsa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xvfoguvr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yzzgqwds.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cxmetyqg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ovyuibyh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zxqjmfxx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmhmespv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kzxsnykm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vhccwoef.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ekfbuatc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uwhypnbh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2azmuiekn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hzydkymh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iqamkvqy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dmxdgyie.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvbbpzs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2idehhvav.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lbsbjtwi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ohmzdpzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xssnnlya.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mdjsfubq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rtqigvez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lntvszrg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zifxnfmz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2utexkzmi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dvziqtuw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ydsobbjd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2akzfszrt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zxjmbuyt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pjmkmzie.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ftzwkvnt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pzevkcyw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohwokysr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dsztvvos.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbeeuvvc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyqlkmlf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nwiyrmnt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vchviumf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2myxshosu.html


<!-- 参考信息 -->