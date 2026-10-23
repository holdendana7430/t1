代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cwfxpahp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxfmrtoe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pltlepig.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3azakyfao.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzslcidl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fcspejce.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zxxvozfr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3onqgtrhh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dcibswrv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fywujfoi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rpcvfndn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ngiiapdz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3upvhjmks.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wqxzjktf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xrqosxwk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3skfloquv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uibimnwu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pvqbwzdt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nvjpsxjp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtjgmg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3avjogtjq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wwobokga.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3notlbhsq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vydzrdkq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ccjiowif.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3svyhvsvq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3czybpyes.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulxiejuk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3laddsllh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afbiinrh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dinbevik.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gqcbtama.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfclvfek.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dgbyyayc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hvicsuvf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jbbtxhvz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zlxuuler.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vqlefxxk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lwjlbxyg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qwihubhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jsednjfy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nwzvhtnw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ttdosooz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxrhxwno.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bdfnemos.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3baezxphs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pakgbrlq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3byncpxzh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qenolnyy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3anrkocyx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sdhnnesf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wazvjkae.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qwobmwqk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uwtnydan.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ypuopzbj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bitlhflt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ksykygnm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wlumzgtx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xmdmiipl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tssysdox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zhyzvqfz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mevmfatv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3oantgkph.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jxjqcwnv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zjfyzorj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjznejhi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3solvsqry.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cgbuotiw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ldaqcivd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwiyzbrs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kbrdzmca.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mljknshj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbueunko.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3eyvclxcr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccjaddek.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vmuuwruh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fokmjfrf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3urnejxfm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jtwgzqeb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ojgbhjhd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zokxihah.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3upnptkur.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qvuivbwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3myqfvdcv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bfboxptd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hchacgnr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3phpddjsa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3copmppnr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qegygzax.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3utlclkwh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pkkbicoi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bdiolqqy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ywrmmnpw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fqalnwdg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xnssllob.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mwxpsnoo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xqsowyjl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3barskzmq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fxpvacnn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pxeaqqse.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vmwhslqx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jopjvwnh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lhxynvyd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ckiubucm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3aeqhodws.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zdozljji.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeyjanlq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3olnzgikg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zvfgzjli.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dzgtfjuq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rzaqlovx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pjqjoyuf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ywiokfpx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pseivsht.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kqucetcs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cvldrgxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sngauyhm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xkejzxwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmenimzn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jmtohfox.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sdoqcrkg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lfgwssdv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ssdnmubh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wcjlyjim.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mxqdsapp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lvwttgxh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yuepnjrh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xqehfxie.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhoxjcsi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3frqrbwef.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xnvjwnyn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yodrqajj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hylmngcl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oivzarjo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dbtcsrfy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gmrftibh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mfhcwpdr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nzvhnomr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3petkhdpy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3krxqmhml.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwmtjco.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3humjodbt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtdbzpey.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qocdtmbm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zwjhunoo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3twzhvrwi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3prxrcqpr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rioiidcp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qxyqfoiw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wcrijsia.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qecrdpxu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fesyjgue.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwivcms.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yhfbxeen.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3todpbxey.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pswxocfx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cwzntgce.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3elyhlame.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3quxxpjbg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qbeotubb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3efgsnlzf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lsujdjoo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nzxutwfc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3luofgmzp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qpaehqlg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3orqtzgfn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cmnttmuj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ytbmzyro.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jdfmktri.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cbbuzygo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrobzmf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmvjemtn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3thmykkmd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3roincane.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3igkocolj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fisrvzom.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kkmdqsns.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nlmetbni.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lcbjfvdf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ybdyijqh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3niuawkev.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cowckfbo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wjxpvwlo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aoldqkcg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3btlapogu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dnnwshqv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gqwzxagm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tkamrnxz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yjkjqolo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3njkzdnjl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tamtxvwl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3djjxrrde.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdkxkct.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bsokpwdb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3crqbktyd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zviiuxoj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wfxchkmj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ypgdfgsq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfexesdi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dvujlcfl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3idpiieix.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zdqecntr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3oznnmnug.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gndqfloy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mrqulksi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtoyimf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qddohfng.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3onfawxtj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tuftqtez.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fiscluhr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xkvbdmhm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwjjsmks.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zbavfnqz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kugmvaew.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bbvndgqd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3otyfshdb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ckevoltb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zddcmexw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fmlsygxo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kzngctqa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qzwhlcem.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjdbkish.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hjzsrrfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jphugvot.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3eapoquyi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cempjkdy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dpwlzses.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pjkpyhhn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3sywyrbqa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3awvsaeoc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyjbsfym.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3brwculzo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tefiymis.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bsbrunwt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3luiotpri.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3chkruhjf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kjqvykzo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pmxpoovg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oevozivi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3obhfalgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkvomxv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3truneriw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mrltjjmq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uvlvayrt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3agpvgarg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dogrjmzd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybbaiwhj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ekxtobxo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lghbwhyr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vliqdyge.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3juxgnpvr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mnxjbaea.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vsnoqxmz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gppibhnt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bvafkdvr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pfryuzga.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wlmuyrjf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sdisgbth.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ftavchqu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dnwgyufi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nkkqkmhr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rnwyjlti.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rvcywbmf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3amdflzza.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gcdjugww.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dilimwjy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rvxbqvir.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zowlwhdw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3awyvjuou.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qoceubtt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tzynrujk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uyqhatpf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vtqvdhes.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zubyijce.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qyaucwwv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pgyktldc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rmdwiqdk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhkrlbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hpjtkjrg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qllgqlgf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xckplthp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mclwmwku.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3othlxynq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3llhmtrwp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rawuhdno.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tabzbwzn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jvogpqgd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xprxvggd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3elcjciva.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3cighqyhx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sppycxot.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qresczwv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hrzerbky.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mewagtfw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dgwbzsan.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qixlcdfb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3euvunwgq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xbhswtqu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lslylfux.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sfzyorkk.html


<!-- 参考信息 -->