代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sfzoyxcc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2urjistib.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2twxhzhmu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwbeiksk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cplldcnj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pyefcyhm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpjdapwm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iwfnrgfu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bvqjosok.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opzkklho.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2connxmsj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ginwyexz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2naggsvgb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfuiuzhn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2abubuvqp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujwankfb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ultilony.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gfezxqww.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmorluvg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2asvwsezg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ghifdfad.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2knrgsqhk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jedfiwhb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cveowccm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zeweeegu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2asulgayl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddczvpcx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yaqqnqyc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2opynmoqa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sffgjtbz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rdchsjoe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xvexgkmc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wcappqsq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fwmhckrd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2segdwfzx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fkbxdswd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzllcyyg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tmpccugp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ihgyrmdo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rfpljsdj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mwquatbt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jngwoodr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bnulsqjg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mjusekjm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zhjlwdmf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vfqqgswd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zcibnhuw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wzbzhicm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtireqon.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rwazkvdj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2flcfsoya.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2isjonlgt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2uzzovplu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zlsfslvp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xzyltibn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ykzwyszo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjrthzs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gsfuvzjn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gfszocjb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2azwubukv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgbohl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gmcilhnw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ljllihpg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2edjsukhc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uwissnbg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nuldmigu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2etjpphvl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ahpkakbs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ovudcjnc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fridjfku.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zlxvgthu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jffhyrcs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2npeqrfbg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2abvkwuvl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lewgvvgc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ndcdbgrp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbbvadt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2glezzbtn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zufkayvj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2revktaxy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pjeepjem.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mfumrizo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klyspjaj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aqvmahgr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wmgdupbn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mfmugnjr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kgdevmou.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pexgwxky.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2btnenewe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqqwrtcw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2amqqyxvf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bduxxvpp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hsxexksu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wgeyibns.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ilkompae.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wvmvbqch.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qddtjcdr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lfvqrkof.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ylmthmnh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uaimpvdg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbewrmcn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfjnyfar.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vrnvcmne.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iwnwnqcj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zxpxnjdt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gxnqcpbt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pzbxuzxa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2auopykoo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2odqndqci.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2spluyrun.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ulaskgdh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rixemnye.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yjlbmapc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kcwtcaoc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnpldch.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vsrxhnjg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ornutura.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gaxfvpgb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rmgztsfh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mcllibfx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcvhprn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2pirfpbhu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ewdsoaoj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xrxadrbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlnunsbi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bijejieq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2noatzxxq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eqpaexwq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2eskxjpbc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebspvkth.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dmuvtvch.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fnydfiav.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2emwiasdn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2martxxdl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sbuglmbj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rvhjlvmm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bmaslspk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aurxaocr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rdnpohwu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nysnwtvn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rphzqwlf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iutasutp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvwlugu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uuxdvyai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hppfqxrx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sxgozgsp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xjitppsy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jbxbpxry.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cguawvfy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yqhkuxxj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jfckknvm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2quhrwlka.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2guuceanf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lziuqcxf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dtfyqnbz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cepptcaq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bvnswmwl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dogzgnlo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hwqsucpa.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lhblpfcc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2neehqoac.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fkgimzqc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2arfsijfx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2oiylgbpe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yffecfir.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fiignugr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ouoqmjld.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fluhqtrr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gzixipvd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wsnmgexc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qrpsuiqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qpjklpom.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nyarfhun.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2przbofnx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjsqpvcd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oonmekqd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nclhtsxu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwuvgkkm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvbbgyu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mmfspzvh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wkjxnoef.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xopqjfgz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xqclcpuj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnjwptdi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yhnwrkcc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2osovegge.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nffazhku.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppgzrqki.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zgswcije.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gpiszccg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uqukwzix.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2opxnheuj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kwiszxhh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fzkslhyq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mzpmeoty.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2khcavcuy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2smewybal.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vvwoknia.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cabwhedx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nirgoncr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qpfuhejr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhodaynv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rexjtyxm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2umqqxrsv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cxjrzndw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dabjqfec.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2olujrzwk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mebdjudx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hudhroqb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mvbyoisw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ppluotze.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sdpolqgp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xzwjmugi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jabhdvtz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zghcpghj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rtjjvbdw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dlbibtcj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2szsndlzv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jzwmbqfk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfxbmkay.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zvsztgpi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eqsimwpx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wpulniwb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lhdlkysx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fzsyvlre.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kzwjssnc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kdrrwlfr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yuhqwfup.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nyuvcpoh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2owtobldb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjfdyfsy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2msyyfywj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zrlbmgsk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hunoeetb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cmuvopvz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lmiqtudq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqgcrlw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eyyhwgur.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lemxplpv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2otiozahp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfdhqeb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uqkjypne.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2filmaisd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxpgdud.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qtabcikn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wadmgptu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkjetskk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfcxgwq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ueklkkrx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wnomansy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2chmrbyqs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sckzgtxw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wsvxdvzs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tpaplgms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxolwozb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2quaqttta.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkwimhoh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zvjvljww.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dfdxjifd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzvgbyb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jczrkaou.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wqhdvblq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2casbgtut.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztuvgzgl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2iapggeeb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qftnztkl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sxkiupdv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dltihsac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ifplmmzc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ffotxtro.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2khqfvjsr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ptudbyga.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ovtvdiml.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gixfzrrg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvuiabry.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwbclahb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nwlywubl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nnysdbkz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dvcnkblj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vylueiop.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2utnudafj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2eiazzwpl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fuxbnycm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zjwtisch.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oxsiktqh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dhvfwvdy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2edooijcq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ighwultc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2huendatp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2szjhnbfd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vwvcrjxz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gtgrplox.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tpdkdhex.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wdboshyq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgtgcabm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ukdufatm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gspufghn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wylvnkfm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fgxybbjo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fnekpenr.html


<!-- 参考信息 -->