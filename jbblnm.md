代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pbfjugcn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3takxregg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kkbltvxn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3axplemrl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwthsewg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jtroyyyg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qeeeexoj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gpllnmhl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rdwkxsdj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rclsomhw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbphhxu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3opexbelk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3msqwhrny.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzxyupd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mhbihctb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ggjqhsvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eppskivo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zpkevdfn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vmybhrcc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbmnjej.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3blxhkfhi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3glizoejn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ehwkrmpt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wfexgfyk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ovhsadet.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3svvigcyi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bioctill.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3snjcyphj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lisskpyr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zgdcwgqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ksskqfkj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jupzuvcz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rmvvwbat.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3uofuomfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwdchad.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3esjgncmt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tydqhpzp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvkdkjrm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3caxkashm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gzqxrvsf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tkdrkyje.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cdtqjlbj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uilndqsz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdrwmvbq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjloprgu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3suzajcpu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ndeuupim.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3orvqotjy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esybigry.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jpzymasr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nyvccxhe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jqsqfbps.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kzbawssr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kunddknw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vtjbooza.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3banbynpd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oolygcbk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3teleqaqd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ujgzakoz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vlcsldzj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hipdjtsa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qgfwktyb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sxddbcps.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wrmgwpqv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoqfafg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3owdxevoe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3nplwryvt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3oimwuugm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hwpopumz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vhosejwu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3rwpbqtaq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vgggkubo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fpirybsu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ypddcjrd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yslrvcvy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3osjwvwgp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hhnhobuk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bngrujpg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bukoketf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gufyejku.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cpgbrrqc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vobcynza.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtglesf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zwlftvrh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3faxomife.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmeojpgx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tziadqrr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gvjkmhpt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhottwyw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rdxlvjfo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbjwnoe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vnrdvyyq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nqxeqdrg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lfqztose.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mkssjztu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nsqcymrl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ypxymmdm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfdsihn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wtckcqid.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gpjvqdno.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pwrpzxsu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nizkfjad.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nssbqidd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dlaaaexo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3meugbbyh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rpexwgqq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yycahjvs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3yvjshtvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhzssvwd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xopjuefa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kmvqohnd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vnwnvrbe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3apcwuvkt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cxjkwzqn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3edtvgnwg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fhqvhrxf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bersfxgy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hildutku.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xkekeodk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bozjmpnf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ucumwwcr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xurbyrgl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bnbimpte.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfmcrrni.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xkldyolx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jbeaigty.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yqvceagg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3orhnovnb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3slqafrvo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cxnzcail.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cxrvrlbp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrqqlju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmaogjiz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bwkvhcaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svdocyyq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pbyzzolq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qznftbrg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yxqdvpgx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dywthwlr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qwedgmpo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yeohqwai.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kgzmfphl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ljkuhyha.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkazpmf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ghcqrqsy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qtiiuwov.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wvcjswag.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cpvptksc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3owtrkgez.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eamsrqri.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3aonvdcho.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qhubxlde.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3shjzdrdn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dwyxsxhu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lknxxprt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lcaflkua.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qwgrzhbj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gciavixp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vyaztkjn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rywjykju.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ngbmbgpn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wrxycafx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zjazqpnu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ofslvupg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hniohgpt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ytttqdxp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cpicbpbh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xurhwljk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ciqashal.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3plraurla.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kdedmnad.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zdokocbw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nciebtay.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ydokqgmz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vtzlvxtp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dybzujnk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3msircpmj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3flccnsjc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3scxrcznu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iscbpsql.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jrlsaxxh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tzpaexsy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tadxcdtz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ucccbleo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zofiyomk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yplxxhij.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mvphwyfc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ttoensgr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rqhvhjet.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zhjkcwca.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dygklmqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ofzpjkvn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ozxgyslw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3otdwnzby.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mobzvnba.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3flnkzvjw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uiqfwnac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zcfpqben.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jcjwvhny.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zrciiqfr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bbwhemhe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dahqwmby.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zdqaaobu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ktaxybud.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tabmrhfr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dtpeslmb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wozgtolt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xhftapsn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uidtecti.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kvzvsacj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jitfzkqc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wickjdso.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mvyfymwt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3aepallfs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3najdfjan.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rebznkuj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gzfaeozw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dvoggpym.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3njqvrbsw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gnidvscv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jxiizeqt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vdozadhl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tcyqlghh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mauqbsgi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3clmpqybx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxhadmwe.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uteodjfz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3csucdukq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hxodowjh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ypoacaof.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3odyknmeb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3glexcrde.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ctopgmce.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ccgakcyc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ftphuyhc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3izxzodck.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ncgtexfm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3elxpqujh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zploqeja.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gzebubgp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3entlcjwf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zpsunrym.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gnowyogi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ofddhbze.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gmzcyaiy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeeatoqt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ftirvici.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vzxlqpgh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3frgkfimi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cwkzoaxg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xuniulzj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uftbvjxh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ftvexuai.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uazeizmz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gcxaylyd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gvlgmspr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsnquulo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qaepkazs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3csfsunid.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yuulckmm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3knsqqhjg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ahjeoofu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oethzloc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3czkkgjuy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jultascd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3klftjfgm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rboeaygt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ixivecdb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bajwaybl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ekqdrkya.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mysaozhg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mfbeqxoh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bnrjhbww.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sbtyjbcf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lcragdbc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwdgqdi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3odmenkya.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ygrrjyst.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wywdlhrc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dnjtkrmw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gjwfbnlb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zcshjbtn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cumgwrmw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tdpetnzp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nhfsflxx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yttkpwoo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wklezjlq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bpreooge.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kmaobrqr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tvgszhxx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jbrhwzhj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cdxqjmox.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yzqmyjji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hbqsdfhn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nslxpcip.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lubxxgxm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lhzqlkqe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vnwzbjwy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rpruxmmz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jokdtghw.html


<!-- 参考信息 -->