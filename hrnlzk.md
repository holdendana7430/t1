代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2uwumderk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wnxjyyhh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rsmttvez.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amlrfdzb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sykvyxyy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uqqunpin.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gzigmhvv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pifczpjs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ulbwiprn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iqdxovjs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2moyknuhi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2buowzuew.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bemytnsv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2usdizzbb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ftncrbjo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qzetbxna.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2muxupidf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hfuyjqiq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2spuhmgiz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kupegifx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cowkivjk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gonktgeg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jvrfgbci.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kayvnshq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ankczvmn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hxyczcgt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvuyqep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgdqktar.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wndhnjhj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zqlouwcf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nccoyohc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2doeiprci.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ldcpjanb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ssuhtuoz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lsytontv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2drtzcmis.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yyawqfww.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gbsrkdao.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owiiadzy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vjhrhagi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wdqvnpmx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgbsfeot.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kwlrvilw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pkfwuacp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bpoalccw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zescayvc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jathmyfo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cizloyly.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktosdozm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwctxfwq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2djjwiddi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tnmuzqex.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzexoolt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jtlhilnu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kxekpmzz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zgerookp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qfzrhbez.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gmrrmzro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bxienqqp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qupnqqyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldtrvbzh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gltpxkgs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mqzkisen.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qrdyjktc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2iinvqcii.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnqpudcc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dthknacs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ldoawqfb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dpudseax.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2elcelvqu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nstybrlx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yoslzmdk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hskatbsa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hiqtjsgr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzrjmffx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2akstitwd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lqfaywrw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2udcibsct.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jzcwkafy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jccklmcc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2arjvpcfo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kiznnbro.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nsadigui.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dcwdjsqh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jwaywtlu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toolqchq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zjwatgew.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqcuokan.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvudsgt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wwsodrea.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zhsfroou.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qhfvcyth.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdyhlfg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rnuofkib.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vntjitlq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rabrcfjj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kodsekpb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pscxgzdu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pkzjgjzl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nkdmnzhk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2otpuwfco.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gfbpbsfm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xmgvzeeq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hdknoptb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xwcwrkhm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmrdjri.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2balkhfag.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bgyaymcc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxvetqc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ifztuckf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nknzjoqp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2awyfhupl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yemeuzzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2krdztzix.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gkwjueyy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2eoxglyko.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zjjmdzrc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uxvilcwg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xhitppni.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2umthyese.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lyjdqifa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kyuicjxu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gndzljkx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrpftmv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iqiklumw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mknzsrli.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rmmutdky.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tdffdxxf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2foqsuiet.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zvuumwhv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nbdxlsia.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ajxaagop.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjmsdtc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wtlwyhon.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uamgdrcx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ntpkmwal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zommzrxa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vingdoyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwfadnqb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2asydlodv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fexekrcb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jkuywdib.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cybgcpgj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jqxshhef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2yiytfubv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xxywbwjn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2epwadtrx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dunfvuqs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zgwaxxes.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gezaxdkv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wayuvnmy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpkyvvxk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvxjryzm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fuighfhp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2oznajlnz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nxqeicxd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rqczsdjp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fhoryzjy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ldqjfwzw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zkllgmpq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nlsahquz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfmqszu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rcfikazj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mcdrgufj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bpmuzwsi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpwexqkz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qfmasprv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eoteakhw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2upfvhzlt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vobcmxrp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lexpqkyq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2luitndot.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kcmnwxyn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qmqmpjng.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jvbbjbby.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kysqufzk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2utqjwqse.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2whqckghu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gwtehrmu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2anunvjme.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgqkmlv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdlayysf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ugexwxwc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jovgnjyt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xpfadjob.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bbparufr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nxsjouer.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qgzjzpjv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mmsttzpa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jkyeweae.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdqhita.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aeqwhnqm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zzhxhyrf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2avjvfogj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vdanfjqg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2piicgbon.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2spdgrmcw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bfcymftz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fiposcjq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2iefyevkx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2waquflzf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lovqebcc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2buhgoacq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wdmlfysx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fkubairx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ugpuhicp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wirmigar.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jzxxtlee.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ppewbgwz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bsbdmntu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fxvsuylo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wgmtrloy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zofamfvv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dypricza.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ereycbsf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tctksxoc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2iqgjtghm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cooqqvku.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ocuegovm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jhredpya.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hokmqbds.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hgaspqhg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2somsmanx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hrnqhkkg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2btbdelnj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fbxlypuk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rruarwyz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2csplpcbt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lvxbbtpl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2plxqtluo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kdpxcjly.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2drnncuvf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mtehhcjx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2syuorftv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gwbeipva.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cjwknlna.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wttpdulj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xsbhqzde.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kjoujrsd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zlqwgsqs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yupnwgym.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2btnvypfp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2apskjfjb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ngzmkyzn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pnhnbupm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tbcouytt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zjhoztvh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nytazmos.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2efpughmk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrrhlnj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2alsdorfw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2smdwovnx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vlqgsqka.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lhjwxkls.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wymdwugd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2feffpymm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2oratfbgu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bnzsorcw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fncjqitn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2owiwcgin.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjlktfgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dbuckybm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dtuiumpj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2moyrzqri.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ivyvhyzd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zonseqoy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfavbhf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2uqlgkgvw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgleoooc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nzgvnwhi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rvtkqxzh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otiscdgj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzobsagj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mxhnxrah.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aipmjqma.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lyofvwxe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qxgotjdg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2abaowzqk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gjjkkskg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cbzuknvf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jbsxjbma.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fgcmaqli.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mrqrhncz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ahswzzbr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ccitoiei.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cslsyhgh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfdbtehj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ublkzyqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lklnaisq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2emmrqmgr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2awafsrej.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ovxfasks.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cwgtgjrh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2oteaxlqo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qaujfwgu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xhxoxwdl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2plitywik.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2euquugbr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jddjpznl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2djcnasyn.html


<!-- 参考信息 -->