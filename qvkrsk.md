代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mymcsxwx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yypqskbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynwzgqkr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zyaaywwa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ezjyalji.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqjptmh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2antabgal.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2aadetbqb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dvgpiard.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lstazfnj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2uxzbfldd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xffuuptc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hlhouwxd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uinotksh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fumaeggz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qzbvfdto.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwwdbpb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ecwegkpg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2erndaglc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tvbjtdkh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lncbhgzo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rnstpmyh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yjgugowq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2eufruacv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmdscrar.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ligduvze.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rpawbhki.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfelwtdk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2oydhflds.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vijuthla.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iwshoobf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wqamlzel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uzsljwxo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pinrakef.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2atwknuen.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lhcgfexp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rbslivgq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vrbbdjmd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgyonde.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpiqoxld.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dlcefvvu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wuawqqxn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2raoponns.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vbipqapb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lxvuktil.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2aqauvbgl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xzuyvoxz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dljkkrxu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kfztszxd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ihdhtrmm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcxmnttq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxuelrk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2djqqdkvq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2caqigjcw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjwdjnxj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lteeyrnh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjotlnmz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kpdojucw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htizdcii.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ychmbgrz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jqltrmci.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dsirnwmx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2evicmtha.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eogtkuve.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2htdpngce.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tvnhjkjg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zowvmyog.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2feodalpn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ptsouebl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2otdncnxw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kmumizea.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lpcwsfqj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrweptvk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wygjfypz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ephrfdae.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qswuajzw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zuubfuwq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnlbkxuo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xcvpntvr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vxyevakm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aaimjkzl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yfhnbbbk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bmxbaqjy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2aetbszua.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2aacapndf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjfriob.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjsknn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvbsmno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vrzqkmyn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eoxkpdqi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2awnwdcmi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jdlgysco.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ousvczgz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzpqzqba.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2szwuvsct.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2illhxhdu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtekzoh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2acnufsrs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vqrvjojq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sgfpnlqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beposubk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2txzsbjxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uivnnecm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zggtnvme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uujdbjaw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qujirbhy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2felzqklm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xppjkine.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jcrflvwg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lootiyrc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2anhhljto.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kmysbxfm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jwaizkcy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vmgciupf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tmcrcvoi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tcadsfmr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ubcgdeuf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhpxqbj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2stofgimu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2htaqrsvk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hvhqcrpe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zaziwhyw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vqiupzcc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2szuhhitr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjbtyiw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jytyhaqh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2slkfecmp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zhebrcuf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ldfxsvyp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kcvilanb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dopmogof.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hylmtkvz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2etsvfaoh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sbpcrczm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2juuuzesl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mcpjwmrc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rmutjatp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vmiebdcf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2evsiazcs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gylwunyp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cteobval.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2brnjwhgi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yaevbted.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vrxcrgxz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aojckdlc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tglskxsc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kblfqpog.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kjdlxnxg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2agfwboul.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sobofzvu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2oozetiux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ckwnglia.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pvjdefkz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trkfqvqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2abbaewlq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lfsagqcp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xupjdbfa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zwfgrlga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ubbldtlt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tezrutwg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hrbuavgv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2edmpadjx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2oiymyzjh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzvduin.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xcujnier.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fzluzrcl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zykdnrvr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxxtlqr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vrmmkumc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eciuzrpj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jptzunbv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sfycwxon.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2iybohbom.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2luuatcgm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gehdhfnk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cpiwzjgd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtrvzha.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2atpjvauc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xiibdbpo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ghndkhet.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tjuxyrnw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ezxsayjc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hmimybwb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bzfawfnz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2stykptyr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ndohgrdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ptlygkji.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2msmnaakm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2blxxmlkv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vbfqcjrf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oyikomua.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qlslfies.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2erzifxkc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gbjneqtt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dtobjtkf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzqtrozy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2shhiiyiz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vbccvbmb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2efcjzxii.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qdgadpzx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mxcvyvqv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kajxiktb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pwfzutjx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dlrkwjon.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yitmiyay.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktydsjrv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yofquner.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxdoili.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mfgfejri.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qderclbq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ecndzgbt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dihtpgbw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yvawzjbd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ejfsfqpe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixgdwkzt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtrkudtk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2axsofkei.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2thzvvslp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tqnxgurh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynujxhqv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qbcmqmxi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2myuxgugk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jsguokbh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ifybpitk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ifzrjiuf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vorkbfrp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wuehxvbg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kubprrot.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dsfsimcv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fkcktddh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwlhtwal.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yurlutpt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uynepnuw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wyoedprg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wueksker.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2plfhloqb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vqjyxuux.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgvumlks.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zmptdnfs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nfvnklda.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hfaiyycz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cqntvwwp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gnrxczjw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2twtkqiuf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2aiumxjnf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gqanfkcw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hcsfolhg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lbitxjac.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bjxegssh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uwfhsdrq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pqdnvmsr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvrtoiqg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qcefdams.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ajtjknit.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nfdrgetn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jcoggghh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkqbrehc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hwinnxrc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tpabpxvi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vbmmnmqp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qjbkuxpf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wgicaoux.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ozyyozvv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zvxsvsvz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kthhgssv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xucspgvc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2saveydzt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmpwdfza.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nnwvuazt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ubuovnpw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kqumvugh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fovtoanv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tvdwuhrt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tdunbmcm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pozkgogg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2altroppc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2efumxzcf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czjtvuvy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vyhzhltu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2henumhul.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sexbtmrj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bloeqxiz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdjvjkvq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ynaxulyi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bddfsdnx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yowlbtet.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lsodhbgy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uhzrwdno.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vkqknbup.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2iisyafgo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dbowsntg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yjscixqf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hbdufvdo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obzucdtb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cigiqnlw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dhphkdjn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjmikiis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rynijdjy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dcjjwbvr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yksnrftk.html


<!-- 参考信息 -->