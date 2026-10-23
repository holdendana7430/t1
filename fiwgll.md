代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwqwulfy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vgeyjfsy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3regicabq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmqgipkk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unzvtynd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqlhbed.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3huaqltcn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cstghhhh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gkzsjlki.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wjgnmubh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ezvsgrsu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqlbyneh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ucqndngg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fqidcyiz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipdeeoca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pkrqfjgn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szbuuhrj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3knaqqkni.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3laxkjleh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bzckvnjc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lrtyyrpp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wuruftqa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qvhgdodw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3frlhljak.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwwylvzu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kaknipar.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hzaijnim.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3warlryhp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wkpfkhqs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrxpxup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ksifkctu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hxtrpexn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hsomuqmm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ohzgsasy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bespiwfz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jfrtzven.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qsrrzavh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rsnmdpem.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3npdyozbl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmftgcmw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3roymmkdg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ijjkowis.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ajlddxon.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vpxdfuyg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rswjppck.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3sndcxpoh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3iqbhrawl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dtaltkdk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rcluaieu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3txvpnjqk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rtvepygs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kukjqbyp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rcisskgo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3avxzuxkh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lkwmluvh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jswcdxyz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydofwcwn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3osezewjw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3howwqpem.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3frfwnlzp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bntqzial.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qomufjro.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yteodoll.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tijlmsqu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xgcljigm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3afmktlvn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3sfcouwll.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3idysorvv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwiihbe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqxqdze.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xnzjgqpc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fyzbthsw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hntmpawy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3klhunoef.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qscwkjfj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vxxkwvpa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yakmlqmi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ckccfxsp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uzvmddzv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lzuslijg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3solkzdkm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3htgtsxcz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cthjmrgg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qgrpglog.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zeqcdibf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdrhtyd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgpyxsfq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqysyjq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qmqanwel.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxjvnba.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfeketz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fmhuvkkq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yrmxywaa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vijimcnd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3osnkevcn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bebtolsq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hsfubnov.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hhpgsiof.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sgcxhnch.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pmmfqsty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kaagnfik.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mcwiyhxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsyyvamq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ebrtzigu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fnqgnrbo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnfzhqri.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bmrhicvp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xswvqpob.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wmjjjfpu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3opvzwuhp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oejktcpn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ecudhcum.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mlwegfxo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ctnhxiyk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bbtqwpir.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jakhntiu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3inustvgm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3srrpkfpp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3unppcgow.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3txocdssz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kkvlbaed.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bmqucbdw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yylarhzg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gkfcxfvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoohtaa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kmevijer.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3trvfjgmg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3saygdtgg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wnmeyzro.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tmgegfhw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qdzsogps.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xsstvrem.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3sulwslxw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bjvckdpj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tvlmnuqt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dzpfekmp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3eybpnpsw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mvgfwsey.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aixmeuts.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bgvqenyo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ddtnrfmu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3hahpxquj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zqjbulpf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwnwhyx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjejvmsv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3sthuqlda.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qcycodol.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nrticnvc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ckhudmqk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eabobsch.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3whrrtcvh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wblyueyb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ioniwmls.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rqahvotb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3glehdosf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yeydyzut.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ksghylmc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cctiwdsb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jdakjhlh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gpevckwm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uwxxoyah.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qjncslit.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3eoszrjvn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3opvjefsp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3eigfisdm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dtztjbqa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qtpamagw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xmitgzfv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nuhrwehe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3frjckvtu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mhfkeebp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxathxw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qwlnhhcb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nouluwhb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zzoraanf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3erwuleyc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3okthzgqu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3epdxtrlz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kscfljzc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hbfutxpu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dvbyrynn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xnrxlght.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3efaewcuu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qhylzxdw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cnjvzmbr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3blqwjrbk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yrgdnrfm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mlcwkdxv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkoyege.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sbifefza.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ykitfenh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xikjansi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3surcpyxf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ublqmxid.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ttctilrb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xyuxdnnp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ynqncpwa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3elmlmnch.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xnsvodrs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ywsdeahi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3erodjqfq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ydcngyli.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xexpgrtj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mikerbhd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cjkbovaj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dniwkrrl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3brjrgzxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tlrjvrsw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hfkkdzoc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iobilgfr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hkdpqimi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rxblrqyt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vodpdtvv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tjwhhbrs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cdlrsgob.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyygmepo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ghfvpmzz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3caytiszc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3teiyciui.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cqtahtnp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kzjidkuy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3oxsodchh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhrwykas.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vselxzqo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnueihb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fkhcmpfw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yfxjkgln.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3miltzwdo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lkkbjbsf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bznntrjg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ucbdjmol.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ietzdxgi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lhmmtzuq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xmdfyoon.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3emzfaupz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xpcdyflq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hxadshff.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqeiguwg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vegpipkn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pnuybelc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3msbxddyd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hzabexct.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hgaxdszb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkelpmy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3onalaopn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ixlgsxdi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ooczixty.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3koitqjnk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zuorastc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzgurfer.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ytyerqcu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbsjnql.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrqikny.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ioukjuxg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wmkptabz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3adqkjjni.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kgzliliv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bklifwqh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvtagsr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qnaoqrqg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjvkwmz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ngotzylf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ldvvavsz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3defwjyxl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wemtespz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qvbwpmcv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mgdhskki.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mwpdpquh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3odhpbbrk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xuwvxplw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wygssrne.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mfecnjcf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3emkuqpwr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zrwhljhz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ceitqwrv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zkvzoyyd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3letjckaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbxyuuxg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gaoxqcfp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygicolxp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kxmbdexn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gswmpcyv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qbvtyrpy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kabwhvlz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bjbkxaqg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qciigwbb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fvyhfjvh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cdduqavq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hzqwznje.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3krbdznjq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gppminnk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gpmppuvh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3iugjsihq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3autmatex.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amimtbxl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fxavzvzm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ttlsfwmb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3niebqsef.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3watmzurv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vcasthtu.html


<!-- 参考信息 -->