代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dsfxlwfk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3afgjvdbu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apemfbiq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eowktysi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uafuaita.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dvanvjya.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qvubvyaz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sdqjtyla.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlskewqr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gzyosgug.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swagwgwa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pecngalu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vikwayoj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uuamgvgn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3sxiwavxx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mebmsjll.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ebkwermu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fifjsjci.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vtourvpy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kukcytiw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wombussw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrvqxid.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gjlditdz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3beemkoig.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfzmwzhr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dvrljrnd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pwzbsppw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hgixqfrr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wyfwrbpq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yznhehsy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ccvergox.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pfvwumkg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nepcuhfc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlptijst.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3czvbbiyy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dnvhchtv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cysbuofk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nhaysggc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vqbmbibz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tbawncur.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gavogmqh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zjtirrrn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rttgotws.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wyzfjsns.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cpudvacr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3amhnqqws.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nsfcpkrw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkzgwrqy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gigdqvll.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vwfursrf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vlbmzqjt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ffnnotix.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jymtgudn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zyuiyvlm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hlnclgly.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rpqvqkgc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mzyejbyn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rimrkfzv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ggbbcwsm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qtoavhbo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ctpzgvsg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bftcurur.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anhvhohu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hnwxbrip.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yuhbqhvt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bczbkhpb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yotunmuh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fixnoyvv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qojhaobj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxjaygd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bhmjrezy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3dhflrafy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fvtbyukm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3neaoayix.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cijuiczd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cznyjaid.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vjhvxdjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3olwjzkkb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hzscouae.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3blnujcfu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjslhplx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3aylrvdmf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zspsqnnx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qxzjpxdc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpkyqzyp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zekqpwlo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gcbwqkub.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3eloxfvua.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvizrwxf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3unfnttuh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mdukvhho.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wmjesisn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mrsfkvww.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jdsfnuls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mqntflaf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqrdbjwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bpclhjyw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sltipzfj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzofccmn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xpzelyuu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tkijjeqq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mmcknnaj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vfpepozf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cvinkbeb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3szroavbj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3eoipxrdi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bnhzalpx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xorjdewz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jahssqxe.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3diztsupw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woxpzsqo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tksgmagc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3aungzlav.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ozkqduoc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zwpdpkkn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hbirnrai.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfjsayvb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tqqddsed.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ursebwtm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lfkrylsk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nsnluerh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3evpeputh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymdgcalq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfnfbzje.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qprvegeq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3klqdwuxx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uabyfdjm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sxlfpqog.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dsnbtetz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ihqspvxm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hskuefgr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kzugkwlq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yjqzoygb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3andkssxf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkqsksu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ykbsupdw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gqwkbcsg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqygyrh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ukzgcxix.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jflwyirn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oopefsgb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jdzigaln.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mnjxcann.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bsganbww.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bdocwqtg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dcoasnwe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ajqetkad.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ijtltzgq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rpoireuj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nnfyddxr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aoxetulq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yvdljruy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ljvswkng.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xrkaxdpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qnjtftnh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3klsineaf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dqwrhvlm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cqdixmze.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nsoxdxvz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dxoxethl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tgwezqlp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bbidixbs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3traiccmh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hgqopqmk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3skjwjriy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3usssgykj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ynjohbrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nvpezmdb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3oeydtptf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ikhzcgag.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3htkupymp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czokorrv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3klugehlz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fjzzhztp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3aawggiuv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jebqmdoz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vgeaxbof.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kdbsidkn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oqiwulln.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oeumrjzz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mpvgrcou.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3powxdclq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ukfkhaww.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uasnemly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpharzf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jektuybd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqlecmin.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ssylnqog.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgsmvdg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ehctjify.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3czybjdld.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzhlklsx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zfpiytmy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmljdhpy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jsprqzsx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3etxqveql.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3irakenib.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3azeqnczr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3otiunnny.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3karnlzwb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3isreuyex.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmnsgund.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xkjukoix.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3genqgssn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uuirswzp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3chuktncf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bsiibdqj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ifbimhgf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qxahtjqq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3trogkbke.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ufthyrln.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpmhsxr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mgtxapkt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cacbrjuc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvehfkjg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hftxclgq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vnjfmbwh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rmhpcrdj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3yhaczuhc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qedwyznm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wzbsvcew.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuklothk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cxbmislb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqarouqa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3capletxn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3neyttncq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jugqgouq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xebswajh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hikcgbpj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wfbzneos.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dngvmagw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wboqbjiu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rlfaiahn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wivpswhf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jwkhgbul.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uxfpdzjv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsujzcs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wecoiham.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uoxvbwfw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yutyuyjc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sexpxayf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bzzzeygy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tycuonjt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3scjplxez.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhedmwp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qrguxwel.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3owwqjmju.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbdfitsy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ksipdrbj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zztvvzpd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rwihtmws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3khqztgre.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3llgiocqk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tyxjllqf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ujuxnekw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3okrxpmab.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jeluaomw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3tamjupws.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnxiuirh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wizmeuht.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3unmjyyix.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uvykdfng.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hfwlfmhr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ygtollko.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nxqbiypi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3whekbasw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lhqljcjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ixsudfwc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvjyvze.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ybuhnadl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ecnafhdt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sdicwmet.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zuhjpgnt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3txlxzhcs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mvtymfpq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3waovwelh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kzjtbglm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3baquxtav.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qkunyzou.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3eqsfvcrw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kklwpdwg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qrwxllat.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mhragztr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mvwxhvtw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hjwixfhm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3epaxgfmh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cpuzwdor.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qwtodsdq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtfkmrmi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3oaygkajo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mozvmmba.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fnyagsty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lgpidkcc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wtvsjfjs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yysutttd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3exhlbwcn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3irhagqbt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jxrsjerh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofkqlxrk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zwgqoswq.html


<!-- 参考信息 -->