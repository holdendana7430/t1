代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hbfibuap.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vintrgwk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urcculgi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rgnvgkjh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3eqfislbe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xmxghekg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jrrefeiz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iccffkzl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fkfqzcgy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dhdaltfp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zoykrbzr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dtrgxrvk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xpugqqkt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fhixdouq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tlnfusvr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uqwividl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3psvxuori.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wzzddcsm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mjfodmlt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3njpgogpv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qumrphyf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqpqupyy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jzlxqjkt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cjnslore.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tmugujmj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3htbrghov.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uedrkrcz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3araisatv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fttxakzg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wjhzwadt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kersrfca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kkcygdaq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtrtkvzy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lfedemja.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fmkalowb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ztxajniw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hhzxcssw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gaizssfb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ysacyxeh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sqeiqikq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pbtkqlzx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekkxvguu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vlirmecf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3llyxsgmi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xiwfmdpm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pgivwwiu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bwhbicrj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3naizkrpp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lnybszrw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pnidmglt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fkrvykxc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ljpyrnff.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jhzigqch.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qpeqybdj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3suavtlrb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wzteflec.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xanstphh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qxeyuhjf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ugxznpry.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zdbglzko.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3iapdyljg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3otxrldwy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3koqjcrwn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3oogfcsyv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lyfzzsgi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jcawonoh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ijszjhtj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3riikhyak.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wnovhgmw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmquemqr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3suznnjqe.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jvphzdtk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3sdxyrwoc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fpjielsy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljkyitvr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qaotjiho.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ixtlxcww.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3srtqposo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wbfdzusd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mobgtvze.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dnqofvzn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3altgtzwp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqtwklsq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3redcxzha.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vtsrkeeb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3llhkaznx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3slxtqyzw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nczkdmgp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3purjltmu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gcmebtmv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cbbwbnhr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3klqwjoma.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ngnijgjk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zmpaqcqp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3waqqapju.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bjlwyacv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lynsumwu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lnezcrwx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bcwwwoei.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fxazuaea.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cmmrffac.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eilavmdg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vufakpyq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lbhbmteb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ocwpbclh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hpmvdety.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwzosbrx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3owvlwknq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hziuvqpx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bohchijq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gqnoerar.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3geihvcne.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rcvikuvh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3viricjua.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dmdarlcc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vbtylhvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwswonyt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dmwhhkar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwwagcke.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rsbgsaal.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3phbgfdgs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mzdrmpdz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ggnmjklm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bovhkcnr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbkmhaoo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zgpnlflq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iarfvbii.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mbmxkaax.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3byxzpfkc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rpdkmurd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3coqxhvki.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3krojejto.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpfvxbj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jtfeverc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtemktj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ngfwzgel.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hkfllgdh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yctvepwk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3unmregdq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvcftysq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rkkbnnfu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ohyzbltk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nhdcwtvz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wbjkgejh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kjdemvsl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3irzuymzs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3krycnjaf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pebhdffu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3suslfpdx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ekujafma.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fvqfrsnj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qishznpy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wgxzxard.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3puuwbcis.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3noszdwmy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jozugnoe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3azvxnvle.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xbdfurvb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ieucwdyv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3znpwsrvq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jntlbjac.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3oriijxyl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3znciyudf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3luwtrrdn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3oabxxnlw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3izpvtcpf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3evjndyks.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tsqjnxnu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cnppsfbf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dsngvevs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbksrgo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hyeazjsd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pygrszhd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yyeucbwc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bssbfxkn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zkfytksu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3sgsofcsx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zgulpdrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vaoxclsf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3eufqzsuj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vdihbfpp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bcmobccw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lcpxomrf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xkculljq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fibchmsy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xkyzgwxd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3whncoude.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uohjprrt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3agrxqsgn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jfyyxnvd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzerqyg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jybrjapi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyefxdi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xglvdzlf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hartxnps.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wmofrcna.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jgsbjbfi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kkrwknil.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3thfyadnr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hmmgwtil.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vmzwbser.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tvxeddnv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fzfhgywb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yqrcwyzl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lydlrxje.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3utggyaya.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rdaxbdzn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ijugylkk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fegwohqx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3daofuesh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qfrhcubj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtnyiqrz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mzgudews.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lyrawvmy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qltaazpq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lckamclv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ficqwbim.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bvsudthf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3szzcjbul.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xxefckvb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ahbhjckq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zvtuciyz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tukebesj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hsvcfawt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dympmtbj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3shwpoktc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3adwpjpdq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ogehdhxq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3luymyvew.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3epzeymzt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltyrbptj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyjkgbmi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3okececix.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3iwavrfsw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lhohmixw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcutueya.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3towitvls.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3exbvqltq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uurghbar.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gixbekts.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unppkgrs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lummqabi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fxcwxiue.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3seujeejv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3smfjouee.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3liahkmgi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tfbqnlbd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bknwuazg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ainkfkqy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cylawhiz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3osidtjsn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ftwipwwm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ldhktkzv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3verdraai.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nbovrvwn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwkaiicf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3aprjinlo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bypnunuf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zvrajcna.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sllpscbp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ydkdgtjv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ijpawobf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lyzstflm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3amushqoa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3warmdblu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3brnqlvac.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncybsnzq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olbiklgc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zozvwpcy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kcixienw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xvwdfqog.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lndhroze.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhspahgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zeohgmnu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hibqkqgi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fqjrmera.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwxutyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3riyxusjr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bvyuqvzm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uioviwnm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3toysebqu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sxpgopra.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qebplhdy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3behsgmcr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jrvkwwab.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qsnhbtyl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3nwfyzqiv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3aewikukm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jtlimwwn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rrrhwnxm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tyflsjee.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3loapcino.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dfglaobp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgohzukq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fsfrvzyr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tpmlwxbj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyxoepdv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vbhbbymp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otimepvr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3crycshhw.html


<!-- 参考信息 -->