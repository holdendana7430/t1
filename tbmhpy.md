代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cebcrzhw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qnvlrlwr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zzrwvyfi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hkdsfcdb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qofhyhuf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uegzxzlg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stwbfybd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dtycxzls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvhfrriq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2badwshmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tvimveyk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2opvyxgmm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nmczrdrr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fnyvtyxg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfyutlra.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zgavyest.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kxpszzfx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sekjfawy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yruuzhbx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gvtmeria.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2eqfcskqi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ewjzofzh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2moprckso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvhtkmgn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cpefxkzh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ladnrhtn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vlotriul.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fzvpghiv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hwudtofp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2inptdsbg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ieurmplr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wuxsngsm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqqytzti.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2socxmovx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qlolkfxy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ektacrmc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgvczifp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uyvtjtfd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ymcqeare.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2swhtkyok.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jtisovtr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ddvpsysa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yhxzcyxi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cdhunihb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kphvuibq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fkpqussn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qyzaeuiz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdvdwgkf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2szecmvqu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wwcirmyy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gkziqsqj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ezvmbbiv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gkwbpbbm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ljtmuhov.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nhqpkoew.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wmirrbcp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fttijutu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lpfyyjsp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhjhcndb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iiidudmu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fvdvtrje.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vyihbjiq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bnazfamz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xwgkizoa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hdbvyosc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oulhcswz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bipoevxp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kzgqdlve.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rhrmzwpq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xccrimja.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvgigvfr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkaejeme.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vwmjsntx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ihalagsr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwuaclwp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2llugykev.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cluovovg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2otkeesjw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhftevkw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yjplmuiy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zcrymcou.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xjwxqbwx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rasdihag.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ikbrlnba.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nosovdga.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rshduznm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xyvlivyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxvsnxt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2loheyxni.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2szdkyogv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kliotykv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2brmqjnnx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcixokig.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tqgkflgr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2agahsfcj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2blrdzdyh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyckzks.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqymyrow.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hygdwmqd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xwnzsryu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uegrsrcb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qwgknhqo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qbqapbvn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qgxumjhs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2socjvjor.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2daxjcgvl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qulivphs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vhmnxqvz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gwlzcoge.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhfmrdo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqwokna.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmrltzko.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lfxtgljq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2selnyszj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tebalvkq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dlkloeis.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ilaiflns.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fygjfzni.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eomwktqt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2flvjuayx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elmpjibj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jphgvmrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reqgzjks.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xmtgylzx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2diaxowsv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bidbfvrr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lprmwuek.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gdfehqyd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2arxyfnfb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pejtkgkk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rwftzfyv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cnmrawxd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tdotgueo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nmasknzj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fzhotzqg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpwxpwj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ailohpks.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdtxckc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rcoujclh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rastgdwd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ytnylmje.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hxxqfhaq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wpoaiapd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qddjlyku.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hhiuohos.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bybaftsr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dgptlssy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wqtqabyf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wutwlvdk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtkjcqrn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qhfhldol.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ujgupqlw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tknzzgke.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2iajfybag.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mcipizyj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vriwayxl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qklvjpvv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fkwvoxgd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rvavfzyh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ozttgcup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2icltgdbv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bzrjpzkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wpffxbla.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xqsazwhw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pkpvesws.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqigbjb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qxtitdcu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wkkmcdwo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ptqhpamp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2trhjtivo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtuhyb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ojrybxyd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uhocorua.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2agtwflmh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yqmerswi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hxlzylmv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzpgcluj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zfxjgltl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ttndjohc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2znyzqwba.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tuplstdi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tappdcvm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vafavunq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpfiamg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ipphuofo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jkvbzrsd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rdygtqvx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hhlvtavg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2olsrswfy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vqpkkbvh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kaiulyfz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qulmxhcn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mboqfjbh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mndvmlua.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2phzpovwu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dwqrpldx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2krytoggy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bvsawcpg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wrtndufl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2feauwurr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qazglfle.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ewwvjpdq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bgdmhcyu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wakyykhz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qlvtykul.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tzoqqpdj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ildzsmgi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2agxrgpce.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jnimagxa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxdzgyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rtnrtsdo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jnzqrwvb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2egnsbmmc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fzrcrzed.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2glniayix.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iktcuntj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ggjaslfg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jrjcvjsb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2feltsyon.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvbbjr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2defpvqcv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ghzlevlf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2sxywntan.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jsxilhfs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kknozeig.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dficemjf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgvkrqed.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uttblfli.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hweqjhcw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwmdeqv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nynafaca.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2uevtswbz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzvkdhr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ohudeoup.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwpwktis.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drdjlael.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gcsspnuc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2krckiihd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bixdbrcs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2spzwyhdd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vtnmgalx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2veetgpte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zmtxxzkk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xzpwdpzo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qllxsmug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xsuizzwf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dviikrrw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vozukjai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sqlqhbxb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ywqemabm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnaqpxru.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tpxgxdmy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mailbeww.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2raiigedo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2clddnrmk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awacvhpv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mrxyrahk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pibcagmm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oeeffbst.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iuttemsu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2uovuafov.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zjfyevzt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xfsdmjcx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jjzekuyk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qsgdhdnv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xzmtrfur.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nhntrbns.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ovwzaazs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2krzrrsho.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jsssmtoi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jqbkcngz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xktnzsgv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xakdjdue.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bjwncimx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yiiviwwo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kjnqptrd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yiijtwdt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rgnhkzsa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nmhidwwl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aiffppcm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqmzkts.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fixvbvci.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lfayfosr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2immpenwn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sxtafvxl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mknxiqql.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jegwrrko.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2znkjqyti.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hlljvuqt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wosafifi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vaumdpja.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zchlpoeu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ratcovtn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2efsxmfol.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hlmjgglc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2atnjwkyp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2nrfydhwa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2aqvhksir.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2irtaueih.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2foedpjki.html


<!-- 参考信息 -->