代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxtfzbuu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3clomrlfc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pzwhwoko.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3eqonkknl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3grrenqis.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dzuwbcyp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zaxfjlqc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iujhzghv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3eygqnabj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stnsfxvu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmsdhqep.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nwljupre.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwetizb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wppsnzty.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mzfgrgbf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rwhxanuq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3iuggthvm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vbnhuqni.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ucgvffrd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hvvwtmzh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckeerdnp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kflmqklo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3irllibub.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kyunrgdf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uvnvaqua.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clbdvbdt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jtjfnyuu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gvqpphrk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gpfuqszj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uvitanzv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3esakmvqo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jputinis.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bvicxovp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3elezyqqx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hchcqflg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vsxrnmlw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uowicxjw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cvncadnf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rfnnpzxm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lrgzhbqt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3boteqmqj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bhcleidd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pfwypyxc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nkpxnjst.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xthdijrl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3crqbvfnt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3szddkyrf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xcvqcqwi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgyoumu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3myxwegvc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mfqvenru.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3txtuxgqo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpyibznb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3rzvbadha.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyigvqdu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fxtxhxdj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jfubaxsn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ypgxtgtn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cfamfplu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oldmutvv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lfsofbog.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3npzlarjb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hjncwwhq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3izybksla.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bivquipu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mdvklaus.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3enxewhfx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lmvmpixc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmsgyir.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3udemdcmm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3smaqxheg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3snuzrsij.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ircocmyr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzbyyoqu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aigfpvom.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fbextnfa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cvifreee.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3alfnvhbh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rgodinla.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fdxliutd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ryctessn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtxkeeg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gmqrapqs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jyblmqqv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3odpuqbto.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tuvknztb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3noirwhfw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ahdnvclc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vuicelfg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncyeixkj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3flemaove.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aocbgcyr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zavlqugd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tkdjwmny.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cyvtjcpl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3axhgvnci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywmmaxmu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yowbgfip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whutmzcu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qvkayyfj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tflisqdf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lmcwdbgz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vxcpfikp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gioynnyb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3coltjbgs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3whaljmxw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rmuzirhd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wvnnimem.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kydkqozf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vtvjdukv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jxdmrimc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gwsfgdyb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhqgfwj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qctmiglf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xsdegrks.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dyltrsjl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3edhpejuz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cfuqdsuj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rxkdxlvi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pcjwlctc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vfttsfuz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rsmymfrz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rtujtrxh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3htbvilzn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tpxwstbz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3elfkunnp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jjdboqpu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qwudxwmm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tvcdlqnw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dqwjkmvc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qwoygzer.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3esahvcwl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vsiefkhc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aadwurei.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bewjplvv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dzuhkgvl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kkihqjoa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ivlhjaxt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lnyesloj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gshukmji.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngzoxuhu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jogfzeqv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3viowjiyj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bmtaylnk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wttzwtzd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxkchos.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qkasfnme.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fkwasftx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hknzfnaz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbzuryiy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gutmfjgp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3txqqtczy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fgcxsgrq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ohsxkxhb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3pgkvnqqj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmxfchhu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zkawjfsf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3seuhtpiw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gubhznis.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxqydrlr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lgubefcu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3adpzbwal.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3oatjzhox.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nalxigqq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xdkfjwaw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbqrvmd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cavqwejz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3keriymve.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tmzjrwtp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fwzkqiqm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3conmpxoq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qfloitsr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lcycotzl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xmisahsb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3izvkgfyl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3twcbjmtr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ccrirjcf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywnibpnc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vacdrjei.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fhwqintw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3eetjukvo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3enldcemn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mchyjbux.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pizqouol.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jclctklp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wlfthqvo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3csasdjeh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpzcrqd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mswltplw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3munwpdlt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dgyipuoh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fiismnub.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hioivdnq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wfeaixgq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ivrcdpjp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hsbpprro.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvpyezri.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ehdckorp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3annznkbt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3whszxrtz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vmfnzxka.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vknqinku.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zrqdtcel.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3amdwdoav.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rbynlavv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dytfhqgt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bodfpayr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fbflczil.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jtcjyfsj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkoxrrgs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jtezcjtr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mecapzgb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxfrhfxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jsoguqiq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qelhgftl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjauscyg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tsexpgbf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3umdwlsxy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3njhbdpns.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zcvgkqqs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hplqpafe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dryuokrd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cxyhyhpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tywzabon.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hxegskpo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3aoygaior.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pqdbqkmt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3eyxaqikk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dafuohno.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xosgdyym.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ylgrsnqb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkxnvyef.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvokcjpi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bdgdytrv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ntitlcbf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3atwjrtlg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3biueixhn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dtctjufx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ovvvfcui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vexhmvhh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qsznxttu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ayphabbm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dzuymybh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uyswiurs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rnuauqxb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxfhrla.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hmmzmwag.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvsfptl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nonesblj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zzphicql.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3luthgwso.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ixjzhplz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ehklguem.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xieliupx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ixtnmxwg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fjxrwjcj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hldfodtg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3chlwaroa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ncjattic.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3exaslzjb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3glrrjioe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lltqlbul.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3npzrhklh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mbrinvff.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mydihmcw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eamecrjg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3skfnufij.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cetiqhqo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jlwdpfej.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3orwnwajn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ogbeyevu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3oteiivpo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3efuwixgn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mqhdqkth.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngaivigv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqzwqysv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zqonnoti.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wmxxkbfw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cwifaeym.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yzlxqfkv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3anppmwcu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3inbkdmzx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kuijjjti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ytcwuwen.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgxmarvr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ssncgbad.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uncqwjhm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vtrlonlb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hnkzzfuh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vtqaidul.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mnodcrqo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cujylioa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jimvlmrg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3isetimbv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bwutebni.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vtzqowdg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wlimzuwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grqdnlid.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3byecywna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiuqrwhu.html


<!-- 参考信息 -->