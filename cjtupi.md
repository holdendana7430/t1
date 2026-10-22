代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hjydtueh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uhtpphpt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvpkdshc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jqtyqpez.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hmgpwueg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dsjwkdlb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mpfywzuj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fljssvge.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2grwfatjc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xubhduil.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2czpcnvea.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aiormfon.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dehglpgl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uonxuisc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2keoqoojf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2iitosfyn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2mpdinzpe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hwckpsol.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2okcibmxj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sylqiszd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urcnkiuk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2miggyvma.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wbqdroqp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ioojrbxq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dterxcbh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pwhvddqq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2siebjmdy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zeyyevyl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2smqgmzdv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hapjtzly.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ohzpmaue.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vekklwji.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whwkecen.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2enuefpnd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jmtchozj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dcvgcqoe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bfonevhf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tilvcbfv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2krfebmai.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2daoklbrm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjqvatd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ikimpjfz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pkjvrzvi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jnocjtyl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uxeqxzib.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nqoykyqz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jupwcqsh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ddgswgbu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2adebjmhd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dlqdzbus.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2klzwcnwn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2txilhdyf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bcwpekij.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2uoheskfr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rykvfbna.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gwdhkzvy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2edgtmife.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bllxrize.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnffcpav.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ivtkdkvv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xjgysesv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idpmpwju.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uoqbikxk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ppmvolef.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ryninmce.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2odsmblgd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdjhkxns.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mxtujurl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2usfnmvxb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dperndvg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sllnalds.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dyjtjsbb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tssyqzqd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mckamtze.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fmfppnyx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvwjqlg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ecrfgbis.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gzxuhghd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2osqegqmf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2iyacexaf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2plxrthqm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jtbaafui.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iduswbpk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bzvenxai.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgobzfh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pmmuvajj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qnkmjgat.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qxzlnspo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jefkslre.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qjloaydb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2povcfyej.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2beamggvy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gngzjmkv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amqzzlje.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nlbhjzbs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2znhascdi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pejhuwvh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mbooccyf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tggqwpfv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lldjqfcx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qkrtjurq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sdhlgmah.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tcccnkso.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mmwoaosy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bibhoypc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2szioyiyf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pzrctzta.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhmdlxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqmpavxd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2amnzsbfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyqpnkbh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijtxxsge.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mfjlfhfk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mshcdnnp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nehvvqsk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2abjoodtm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2unctlvvz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mxopnmgf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uotgwhft.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hhpqryvy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qonwzyod.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hplwvxxj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xdngchma.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rrvznhvh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrymulht.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xuidntwg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cojnmdbr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oaaargka.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2scrqjhzf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qtysirai.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ruvynpdq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ltfpqmrh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cacnsivu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qvokoffk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxcmqgv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2visowsij.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bnttevhc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2inktzkiv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ilokyczo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ktobszqe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jchvldij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2uubyhtro.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jgxpuvfq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2krodnfka.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ohqoiwsg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pmafyjoi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxntrys.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2eqwqhdol.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bwwiwxoz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wxuqwxvi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nmgzybla.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wujeajfz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kbwdizsx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zhllkwwm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2julhpxqd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mrcgqlgr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2asnrcxne.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2attzjinc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhnrejg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sylpcrpp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2olixrcjs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rubgkizx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mownfsrz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ojoqxmib.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2axiykpom.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wqudfurv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ceocfymn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zirytubc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gthshuog.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dlriycul.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2neawgxuc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umfslizt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tadzgqjk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bsracdlu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zwvtmcki.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgnvqjw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wbfcaaoo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uofbcqph.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ixscsqtk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qrknrwdy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2sakpehyl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2svmsxgqd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwyioox.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2sagmkzlx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmljhkxu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdjqgjnp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tyqbknrs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ocwnxjog.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rzloqslo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yyybtuhj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2obhlpvrd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2svuetuuo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bkckxfvj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2axcyerem.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2cbtfwltn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oeojlqfa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xbakjegq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mskqocnh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2okuplhje.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ckcprxaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pztvaiyn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytoqcncc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oboesfuy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zlbdihju.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jsedqida.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qoodarki.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2smqzqdby.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tijflfzm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ifwzslum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ppervknl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2imgecqyb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nfkdikro.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kvjxfxwz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vtqcwmrv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dumevdkf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wqzbtmdr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2shfkhetb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ldxxqqwo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ltcxzbdf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sedehhsp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hdffmfka.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkekegn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gakayptm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mfkxaqks.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2whicycyv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nzcfxihh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fkowrvuk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2subgdwow.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zgwyceym.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kxtriwoo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gzjbqbko.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2elaqemwm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pvoatnbt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tncywxoj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zzswgdvs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uecvexmy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iungpcfz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mshhfyha.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkqndyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pymvlvfq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ptbkpomq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nlydumta.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zidppgzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbkqtou.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qewgeihr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fuqdkbjs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rlelsphl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ktsywsnh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qlfbxijd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2didynpdk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gwiggubj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lbshzdnj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2unnnzmut.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xilffvla.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2knnabmjq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2arcgdegh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qyhvdyik.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qlowsnwu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zpsjkxmo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2feienqjf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njmmppec.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ikiepsmt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fqucvnmu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gjjwykgx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zlkmjlbh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sxashndc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2inyjitts.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yevrddrn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2unkpbuwb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hrayakjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2awkyodfa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yewxbksp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zqrinqch.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mkfnydxh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zigrenld.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2saostzgc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2taqgmeri.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iblxvofh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uarkmhsu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ullyvyrv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2agzvwwdt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xkdnuuuv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bxjhnnbh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lcemilpi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ygmwuuam.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqnhyozc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxeciock.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wdrgqsyx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2buhbjxnq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2odwoqtxf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mecehirs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vhyjhwod.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ldoqtxjh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gyvxauef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pyjswwwh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oslublhg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2clpknhsl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tyzdkktq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2csormwhp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zydywqzt.html


<!-- 参考信息 -->