代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ngwnictl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2esptccpa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xljsoqzk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2giybntek.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nngieucj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ifggggum.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hylrnrfs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nsmmfkqn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dojjnvhy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jiaxuaje.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2utlkjftg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2iemtannm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xyfcusqf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2icsjxxqg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cgnmzzip.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xytyzrti.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyfekaln.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwcpojsy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hcwxfixj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ygnwqqmf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnvstiec.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kbwxretp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nflukpff.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2sucohanl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zmszwnvs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hflkstzn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kyzozzyr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2noeqzfpl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jignfnyc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tctzitvq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2urnmyygo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ojpnqesh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2azotmkwb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hvtgbzhv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gnepqrxt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2oeggezgo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2soheqbbg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nvbkimgr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yzokenhz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bvccvgin.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wunrjoey.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bnvjbwgx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvlpzoso.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vvfuapss.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mjhyonoz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2frpnhpdd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yguoardz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2riygmslo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pfbehtdt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2giavqhqu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2eewwqoni.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2owlkzsdb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2faxxopfx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsnqbjrq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guhcghpr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zjpulnla.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dyuwhvec.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjnpyvs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iwtxeqec.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ldhrdvjt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2beowufgf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ppktdhip.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcaqegsn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2oshandha.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pksnlozd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2savythav.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bpzulmzn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wcmpufuz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rushjmdq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwrkoei.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kaflbhrk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrlqjxm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vgfbvnqv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2opnauqch.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wgjjgvlh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yqgqlvsp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngjmpkbm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qekhuurl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2igrgqysf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2aongepqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ytcinhum.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iasjgnbq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2azboppdl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ngdkjzbr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2brelrkfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2inkdumez.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mjmlktku.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ogldmqsw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2crxjqeti.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yzqfghlu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xnywbkww.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fxsmpcih.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2idlzfuqc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpumupgv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtlgxyfn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ajmrwomz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xopxfvav.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gbjzdocm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2utpqrmnu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yrkctsny.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vzhhcuel.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jxjxpldf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wmdhzvrk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tntgtwtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukzeprql.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmjhofcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jajunqud.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rtvdabrw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2esctuoww.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdeteume.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rrtcmbeb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qrnmkyhu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxrqpmmv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jirxhsap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ubkzmqve.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svxiwhej.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmaswlgl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wcllcxdh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kutgxcef.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vgyvvlhk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2osrteafy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pmwssfuc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pokdxvtv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ldhseyap.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2klymxdfu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jxjxqnbm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2icwqlech.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mmgwmqlf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2evkabwud.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdbayyla.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkrlert.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cxpagipm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gdajwero.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2egqnbyoq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2muheqyzb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2idqssdhq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ojsnuvvj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2okrriwrs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mpedtdho.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vkclnnbf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rezebptd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jybzpxbr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nsmbotfx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jtfngbyt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qqsunpkq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dtnlrlbt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vfrsonfa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ztyolrvx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rvpgualr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2taavxule.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2yiatokkj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2faiwvnfv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2kjvhofgx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjprybzq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aphlbpgj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udjvlxrd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jphtlrqa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2byraasio.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2esyhagnz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nrotqdjl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tcsfnduj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qumhgbmi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2htueqwxt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2thlpzmzh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2uwnijsjh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ggdodimr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2claiqttr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kzsmxzcn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2owlgxydn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzpbtrj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fnrshblv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pazromqy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yolpldtt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oimxiruq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jyeypfol.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kzlqrbje.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2occdoxuq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hwkonygy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qljnullu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wrjvkstn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2smdtlwpw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dptiifes.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cyiofohh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nrnufzbw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mupsicgv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2diomltwj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ebbrziid.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lkcrjhud.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2szuaknks.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mdxtzmyn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2paisnwuf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqcadf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dietkqyc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wuxfxmds.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpnhkyy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rtywjqhs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2clogjwts.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2sfcmbtev.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jonnpcoh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zhxtlmwu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zzkmsdph.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rgcfqdxy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hywtdlwf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vjiornis.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ranrrnue.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hslrpfsj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qrytofbs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rswfroqu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tvvgcwvy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqdlgioy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ccbqjpmr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2oqsjpyid.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2obshfpif.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qabhlffm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2safprkpg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pguznryx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mtpsvols.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ljuttmvz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wcanzvas.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xrqbcvwb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjpmbywu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bjisnivm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dknpkgit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2msoyyjwa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rwknacjr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2idxfaspf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfokjvna.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xrdjhbsr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hcnwcbdj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2waamlinf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hrnztefu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kpeulzna.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ciwyunmq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cbeagtww.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2inqgoclx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ufifqukq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qpqwopuw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pbcdmzyq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jjlsthay.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhazkht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrxuahnl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nvyxtjmn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jhyayagf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kddwqabh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2oqivsoiz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yoxnuzut.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yuprlhnx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmjqppc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fwtcqdxe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qylakedz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nuxultgk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xoyiyyfs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yrnjekmf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vzrmbbdb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpaeajzq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2peaswssf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2okkftspk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2foufchxf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mfwbtoqt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rfvjdehg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ovwaxhfk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ezuidggj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tldfwxon.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nnmizvhr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2edhulsxh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mumcwdei.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zobkgcbq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2udhrsvml.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eigisfhd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lwujtwug.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2onbdqdpn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nlcniraa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uxqxhfef.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wohpretz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ygpltexk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2stvikiye.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lpssdhdj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ysmwyqkc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jtuccmta.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ephssvnm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mdterxsr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yvphjnzf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kgrrjjsf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vfzndmlp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wozjfilt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ngwerabi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2myzjytcd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cxkoihco.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vsybihbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fkztuadn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mqjpjwas.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rngqtbjk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2flcneqca.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oelqkxns.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2navacvoz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iltxqcut.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tsnwtqkz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puqxucpp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dcmksjui.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uophffvv.html


<!-- 参考信息 -->