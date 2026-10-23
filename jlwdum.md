代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bvahkpxn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujnnnyka.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iijvnalu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsagncbj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdabkubd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dogxumlf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nacoepdb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqscqipa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdecmrcb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxkhdkf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3esantipf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3froghtpj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fadixhin.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rvrtlwil.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fnowpadb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fhlqdlsx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xnjovnii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijoszwcu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlserlum.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqevmmis.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qkrayqqq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ppulyigv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bxcwbjcl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yuzxiptm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yqpcgctr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rejnuyng.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ufezbbsb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aqecempz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ncofbbtv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dalgzscv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ccevorqk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jaxcmmqj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aaduezfe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yygzoqtm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjcxqfs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ghkiensb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pkpxgkjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oxknhjow.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jggpjpwv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mmvrwcvp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bpiavsmz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kogugqnm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qpspvpvf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aufwtfhl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3onzkkukw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pyfmcxbt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwtbbbyw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ykdompip.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyvuswxq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kkfweesp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pvxsrntk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jhpqpabe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ehiqduvg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tuaicsov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wokvpvpj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ezmkmdul.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hjgiejzl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ewobdaez.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vodoyhay.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ncwbuspc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uimdwxeg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ygjncdwe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ceytlpyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mchcxwjq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qlpnezge.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tbvudamf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fxrbvoxf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fvrlgwdw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pttdbpck.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3npculrqb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wvsicjch.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmbqykor.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ebmtmhaq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lhpnkqqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jivbpjyc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qnflipip.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nebivcpg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yvavogvc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rmpxtczw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ojgrgkac.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qihsedyf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kulpcsqc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3glldxgra.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhoicbw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3evvgutel.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhibymyn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3crggiepn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3uwbaundm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qndimadv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ywlzgmru.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcqxxdi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sxrmslag.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eclagnzb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jcmspboi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gfqbcqoj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wtofpspf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3raznfhdq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvbothlb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wvpjwmqw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3faceqban.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ervxblsv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3iaedypls.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ftomvpqb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3keclfuzu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fhkfjldf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zfletfzi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uthnelve.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lflgqzcq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygxmmjwa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rztpwqvg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mmqpmdgh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3asykihqr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cynnqspi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3szyiynkh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wcerbnnj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dtmzgktk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sbsqtpfp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrigvaa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uqgprwzn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nxfdwsaw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3oojfnwpe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nttutpeh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oxowwtfj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rbkflcfu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zlhvkixi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pbclkvof.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bctycxvn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vsmjopgi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3onmhntnt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dhokfign.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ftuskdox.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3brtrdtvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcvnvpsq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gpgztjjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arfblbsd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nkzcdxhn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3iscjbnkg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3aqrunfsl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wycdcqvd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ohklvtlx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmywqpji.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gcdhrgua.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3enozsljq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xxkminbq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3svrodrry.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iumklaef.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3oywyhtsh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kcgjrclx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uuinugul.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kqtuglgk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cnzrukxs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3idjcmsfw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cvziqtzh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fetxwgir.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bqxcnnlp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jygiqnia.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wrhfrfgd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tnppvdkn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ugjfqydg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hlftuvya.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3udgjsabs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nbjbimtd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qsqrwaey.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dygmdazm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3diiuthmb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mgssrehd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rvivdrin.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hzocjwjg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3myrnzfar.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nnaruvnv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3npawxpnm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fkghsokk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ofhlmlwh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ansiikrt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ghjbkfsb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3exihbkbr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uytxobfv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3iizpvhzu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wukziknu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lxwsgafx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3trvpgoyu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vebbcapt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mbnqmbgx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bpqcwnwq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pixrdvuk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jyykwdpe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3twlfujtl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hezuyptl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jcqylqss.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wnzvarxw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bzrkuqfi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdrumcmp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nmvrbmmj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qiprpbwz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yfsrrvsm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkhydjek.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cefavwrl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkdeddh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ubbfasxs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ehcglctp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nlydipqm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kidjwgdo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cmiqedkp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rocwzrgq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qcoygowv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dqfxvysd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hlgijjrv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xdhwounr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkuveexw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mbssrbpc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cfsbbbhk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zvxaivne.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vkfudehz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3acnrwcyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vjpiywbg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vfdqxlbv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dvomcoue.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ktneojpr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dajqfvjy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mjkajoux.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rrlgsnib.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ntzulthn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbhcyhy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tnhxbjff.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mvctuvrw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqsmao.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ekoyqnrw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3omlpyajs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aeeryvci.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3upevhfme.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3nsprbvny.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rzmtixmu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sgkmehsi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hrqrtcec.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yajkwmtf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oelrsvws.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bumvzvcv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmqijfms.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3acxpxvfh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kubgdyjs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ggbqrqjq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmhbttp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xjcrtvhc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jfzhbudv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3plynwvvl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxmsptkf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufkewseb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxopzjrl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywdhtoud.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3oarvzvsl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3cuahvegc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ktxotqmb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eamtmmxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3aooicngw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tplzvgqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qjkaosrh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlkhzqj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3swehiebs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dpxxvkfk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kdonjxmc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rsptoumr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hwyagsop.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nvjuxhew.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akoegjmz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rszedxmx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgqwqpav.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wjqsvaaj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wdbppdkg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3erdsamiv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ewopnsqv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3avlzyuwm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocgheqwv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gkalbwva.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uhnsmaxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pvlivupq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fmwiosco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tuqlpath.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sblkzfmt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qhpjgvba.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cxpxvhbf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gqdegyov.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3psaciprs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwsdpnd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msqwctkd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3puvibsxo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ffjsswgs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aemciubc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ttmanzwf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fpujdnrl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wkycdjdd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sfmoshmo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tzmygzyd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxvdym.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sltxteyb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3auhksyxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ifapkutc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmqxzm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3stwqyzib.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pzjwrzex.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3egnzstze.html


<!-- 参考信息 -->