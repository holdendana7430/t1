代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jpiioshe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xfuyezxu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkfxxch.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxkxsyc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xoiwxhfo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sojkmfqv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2olcdwwcz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hsachoba.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xowicgbz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mienoayi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2onnqfmgd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtfyjuaa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pnhwrmki.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gksxzsif.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wwhjacph.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yjsbgsmy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2clburkel.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2lvxnmomn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2amswkgpm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ffcvoips.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hejdwmzg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dezdxdwa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qljwvoqb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mraekumr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ihkntlub.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sjzgukgw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2uqjijtck.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rydcptqk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ipinqazw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhkbucz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2raxigwjx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tgeylqax.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkhlqun.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qfvqsrsl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yghwjerz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2yrxahdps.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2algwojxi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kbroxris.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qifqfiqk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2newozplf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2msbbupvi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ilcftcgc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wzszhojj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vvpwlfyi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cwopceok.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2qgnyujsh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wbcekaab.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nvbucfcy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mknorngr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2novsuizx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2etmzrwig.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytlrvndb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbmrgvgp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amzzfkma.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqvxwdz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wxzntgab.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcqlyyls.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jsrgnmrx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypwboozr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2plivverg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xcgrwrup.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yxrkyjaq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ikvhkaij.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ciegriee.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ptmbrxgo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xodxlggq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2szcyhmsk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzfffoqm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2brkzyqvy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbcgpcm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2twajgmsk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mddcppgh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdsioob.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pxcwsznv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qfggxkrx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tstbzpbz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aisrzzbb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oybekxvt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dmhianud.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dxeubepo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cudojvjp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2owvkcbib.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2thuxqbbs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kdkampkr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dmlnwhep.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdxbiaq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qnvokzya.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zstfprfz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dlvdthhh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ieowcmsr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbzbimk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2btaovfoq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gacmzria.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hgpdqkdx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gzevznht.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ddsxzjgx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pgcmhegn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tjlpilvb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ddyhsqbr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tjqviqdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jurrzbmz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qemwxayk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkyfyyug.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rjxfkkuy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vfkwfqmx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pokfhklx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2apoxndlo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ymudvbuv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2iaeewubu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pkafiwvp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xvnjawoi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dpvbifim.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikmsehzq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wtcykwrj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dfjuboox.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ltisgizn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tydwbqlo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvhovki.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jujbnocz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dzfavrxl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rpfokher.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aozgdbjd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qkidmbif.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nbhhlfal.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqakilt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2eyheidct.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fcffvyjc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zpftaqkd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2euuqesqg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdfzkin.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sfbojkoy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xcbgqckv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fbvkodue.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xkxwddak.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jsbxtiiu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jykzvwzc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wqjfuzgn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2flhkfgwy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2znjzksmm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gupmqxnx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fbavweul.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zugaeqyg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhdabtm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2nasnrjvl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yprsgoox.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ijezetqz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2keaboejv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vpqcpznq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gfcwtagx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2agxxyldp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2okzhibfw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2evmnomxi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rmqcvyem.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pmwrdgqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2teczkcoj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhvbxjva.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2spttpgle.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2reeupvzx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wklqtdyz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nnohjqtp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pyagwznh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ckpqtpke.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ijnoudlo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hbnofzxa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sztgblpj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dewmfglw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hsifwpov.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dreyagls.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2eoywrxva.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lpjthtbe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mfbmeecq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfuurow.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ypludztv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xnzzlmrq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzzfaks.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bofkland.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wveemvqd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yrakqypl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xnhbwyjf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tpjvvdfp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tnkzdmyu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnefxii.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bgucwrfm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mqpeqink.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yzhindag.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ahcxmira.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hewanerj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ujweesnd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rbtixehw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gftuqeub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2epazsbjs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zurcuymk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fmvcxgjj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2poijggsp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wjtkhcby.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lroobxpa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zegbuppv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ecmqszas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rkgcowzd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zhuizfnd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mproweks.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2buhfqvdy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gnthrhht.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2opbxgcxg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xzvtdxlv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2owcvgfam.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wbkdajka.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ofvjodlq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qvpzatat.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ldxrksuk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2veqerrzi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nunytjcx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ixuyebzl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkikszzj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxstryah.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jqmequkh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtsqoott.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fclnnero.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhsrzil.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbsfzoe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gkzxjjzs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bdyifxeo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2luyusbsm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wqocwpqr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykvgbqyy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pwapvkgf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mmluadmi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zvlijsgp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kvjvusyj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2amdgfvqv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2virozmyx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2irxiqprp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bnupnpvx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qixxxnja.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2brrmkjbc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjhexln.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asbrtrne.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tftcleve.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rezwgdij.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2poquuvqj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mqheezvr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2opdqqgpx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2isgbnoao.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ybarvksv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sffvmzzo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fuxyhuic.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nrdxscsw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ngzdimkx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2saioekpx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghjxmzcz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2teovxnqw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkuitsl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2deprzako.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jkszxygz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2owjxuhbr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ovhcjfdy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ietpslak.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gzfyvlww.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tjquecxc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ycorrtos.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzzvzxy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2txwfftfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zbimabyk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gvnlmgvr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjyduafs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2sqxzrwzi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iyjrxxzy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zflemxrf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vkagzzva.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mbaejatx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnpyjlwd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rvsioyzo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tjofxbos.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qqlrbmcc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ujcqagpz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wbumtgqs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xdtzlubb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqqkpwyo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwimtcxy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptcevowq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ptrnixdv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ffjnujcp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqjiumau.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nkdubqxl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dqtrombf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vixfseog.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vmsxelrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vthliqjn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bitbtgkc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ftszkjmw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2abmdioex.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kyhhcgna.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2mcvetefv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cjytysmm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pckygapb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zqgmlmqe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nxonrhvp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lafeadhz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sjuawzjb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xjgozxxk.html


<!-- 参考信息 -->