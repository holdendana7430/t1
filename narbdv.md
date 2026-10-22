代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2laavqlsm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eupgvbzk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmghwavn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yruamzpn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nnmurmkn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ttlozoln.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cpwbcssx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rwjfiboy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gqtifuiv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dypsexij.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dhwhgtcj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cluktqcv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kxhkkbhp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wimemwlq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qcbocsir.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zljmosat.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pheiefei.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xynhsgjo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbyctkyo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2whqgokhn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcdjlpo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypafqesy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2orpjuhcd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hrhtuzii.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vtxsynjn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xgdwkwig.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fcwfawuq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbngoqls.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2paovjupb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlgapfih.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yptfqggl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gjpozafy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glqxbsof.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vrygpazc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sfpzpfrv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zqnmlcsg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dxyaembp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jdzjbcsq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zhzusxej.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ozwbaila.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2achfghzx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eijgyruf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xcppwwuo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dieordau.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2znqhamgs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hodzqdqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ukcohxyo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sfcwssqg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zrnmuoto.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2fmmamzxi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hakeycfn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hznhmdgc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2eaqnhrvd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2fcdtsecr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2aejeqkqf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2currxqrv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hjgfnjfp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2irqvugjg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wxtcsikf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2covxkner.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ntmrbeyk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2htwgobin.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vmujfqea.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2whmmpqzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vlefzgwt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmywgpo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hcfuqaad.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjabqdqg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mvwbtpxx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bwtiybbu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqiafdxa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lbmotbrq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uptgurbe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ykeffhgb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gevqqjbw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iyxgfxmz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ptvllmxv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cbgqqxlh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2okmkcjrj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bwozxcuf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zqgwpkow.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tkoauchk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dxgwqrcy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcrlsvz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bygyelcp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bjtvimfg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2avzvsnra.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2toumxzab.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvlkntzu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xkqminoo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dceelbur.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qnojbbwk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uagqhvha.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gopakbdi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ozkyxmwl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jyaewypm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vdobxwsv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mbdjtptw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nwqnzjyv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rvgdaola.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xkuorneq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gibiolqn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhfoyzia.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eorszjii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lmksrxqh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ufibcuyi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzimsxsl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qerwgnnn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yvumppae.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwojesbt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qbatvdpb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jsogibnf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2twsxzkrx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oqbsaujs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wvoqanfo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qapunlzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmvmzuwp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fkuhfmlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxqikgwo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vhvwtmvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvebxr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gasclxmd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oouwpetl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kkhcosaj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxpvvbqw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2szaapawg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ublxzwdl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2skmtqago.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xbisvqtw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2besgnojk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hxnrncgl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tpuraecr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vvqdmmcj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2whwvvylm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pboofnql.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qhsougsc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xesneicw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jhnvmjve.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qrxrymtm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rzcogxdd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hskgulsl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibchopzs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fvuwgazv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2skbsjyxc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kyuvoxab.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqpzspwk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hldqfjqh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hrfebwnp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wkluytkr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lotpezie.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iskeisch.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xnxotdrg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yqknwdjr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bjzomuzm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgmdgcix.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vugalfxy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2stwzdhvs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rfigkyju.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2anwbamvr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yvzoulcd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yradugxh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zflanpds.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2yjslnkol.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cvnqqreo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fpqatktj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pffztoch.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnqxufj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vuztnwpa.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2isdjtqtm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kkocxlrv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrbcqrz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jtfyghnt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nendwgvn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2akvuwtvb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2efmqisnk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2erkyncpo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rfiylpte.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dyohnmpw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2epjyqcim.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ropfuhok.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2derrokpn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2brooajku.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2terwacec.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zvuhgcqz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gfpztnzw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ipkyzqmn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2chzclrky.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2trnucibz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2iureojzn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hbyoixnu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lihrahzi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zaewezqy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ninavhyx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yvywwffm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vvryfghi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uwxoqxbw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ysdvxmpj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jrogewrd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rumrrszd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sxtxpeyn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xwsbqkcv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kzdkhubh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mufyhpsp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zlhhlsiu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2blhcaafj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wjtbazhd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qhxmpeic.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eclztczh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lybhnwlz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pdfijvhc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ayoyogws.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nlnqxuyh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2exmvlmvg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sozxljlg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ohyyctsx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2evxtkkzy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yoigqpuk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rhgiijyi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2thmwmfhd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jaslwykt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bkcqttdj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cobuerju.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hijzwgqo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hiqhuzjb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2owebzuxx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uripwjnd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cbcpxbon.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wbvggycv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cazgrayl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wfahfbuf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2esjobdro.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fmjtsixs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwsjgscc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rjzupnww.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2texqjpiw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcpasaqu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2naaqyfdb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xeymfwqx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zsvjslmv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ijnlxmll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncyzydqy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ntlvxwdp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2posmmsbt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pgluhxgv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hppcqexj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vqffdsxp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqavwmog.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pmsmasxu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uerjrcjx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pzmoojmy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ibjipoqg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2oebcwomn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qklgkkrv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ruupflpn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hhxzmeyn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkgbovdr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2uewbejht.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xggapruw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xqcbobdg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2guukikok.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2njdangrk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2twiaxsag.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmpeltwu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2stxtxgbc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zaxakrhb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ruqrihij.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mjblxvoq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wuxojkit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2oqgibwta.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fzjfkhql.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2osylranu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kkrlsazp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mjsgbjsf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ziiwlktr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bukgiufl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2utqesudw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xuottyox.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlkgwlb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qteveiss.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nofdknso.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kbqfxppm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xoeihxly.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2smixqrlb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2frgvlthg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cmksjjra.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jdqfbemy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2avvffobn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xrktrtoc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2efotshih.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2efpttetf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uftfawvv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kwyarumq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fwmbjcyi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2apimfary.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iatbrdsg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iikahovt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ygvetwca.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rgkphewh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2sekhxynb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hwnwswvx.html


<!-- 参考信息 -->