代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kympsmya.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ymfphuqu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ljgcpibe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kvcdxtpx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eggmygzg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kvsotuab.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmwodjd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nldalewj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsxygkbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2locczeuq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ofqyhhzb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yhjemtnv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uvnwtyyj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hvtgxbdi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2egverlgz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkampxif.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhgqtfhr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2debieqgq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uyygzysu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dysdezcg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhbkwgyz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qvlqrzvl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qdtghzuv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2axyzolie.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lvmggpzi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lpvsrrfh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hsiiwohj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2onjgkzok.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xeirhtzl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hkhokjuq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dsyadkhg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jwtjhcrs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2exrxwqnw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2odyeqhkz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zzcxsyac.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zkbtxens.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wbpkpmhj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lgigmpst.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fzkyrpeg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vzbmplpz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ntgeuyrs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2blnyekdm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hfjcceaq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ijjwlhxf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gfatztyu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lqxynnpg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2imkuxfvs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yhgryamc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2okfyoxza.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vjpcusbd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xbwulgfi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2krwkduzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ejencnqy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cibwqabw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hkfpxoid.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xfifbwxh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2szztipje.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2klmokvtx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kldzyffx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vkchcreg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqivciem.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wwzlqqto.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxioahha.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2thcnnlic.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bszfyeuq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ygpcknvd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bwvnkcwz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ofzqgfxu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ckzgwhzz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vvyfpkzo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ssqluzzv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bwmdrghb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gpimloam.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tslgzmrp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wobflouu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2phhpakfq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cldatgpx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eghubgdv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nlkpkvct.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gebqhnrh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chrjoren.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ebiivnza.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qxekswjj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ualrvldx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hzajhayc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ipudyqfj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rassyixt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pdjisyhn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xmemkrwp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnphpyxi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cgckozdz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2noeifdok.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ftgivnwm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eefypneg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kkkvrtyi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxnycuyg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ttwiftxp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnotbaov.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tfiraptt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cydgnylv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ercxjjzc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uxqwgzvs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gkgttlzd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wwlexpzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpnsjowo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pgpuintw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sceppwnw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ibiitomy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xwchwuqg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cksjpmuy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rnojnumn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dyehpeql.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2udscdmxs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eozkwutz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ubrefhax.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fzkvpuoq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqbtoibc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hivbmntz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ehecevaz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2itlllzkb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2juilnitx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zlvfkkai.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wdbnyxoy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2alyubsnw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ubrxvfxi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jqsblgqh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cgtwjlsd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lodqjffg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2umrdbovs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wabexkfa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xwokakxc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fninflcx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nbafbikc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uxtrhnha.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iqaktekk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2siwlxdmd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wcrdmnob.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmmxbpk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lgownpro.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mwzdatah.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mpceovhd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ucywyfin.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sckejazh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ypdepqjx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2konrnzfo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xtclkguo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjdtyrcs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ckcfzrqs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gplbiulw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2reqdmdyj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pwotxwjr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2szbmkcic.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ngckzjne.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfazxow.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qaddugve.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2azhyhcjc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wpifwhew.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vluskzak.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjtjbbui.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2suiaxznw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrymycmp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fqxmbyuv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ppppbysa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kheezpzo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2stfqaqpz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wyrojgtu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rgllznmz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnnnshb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2irkrxlco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fymhsdui.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ueittmik.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gwcjnwkv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2thqgwgrf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2flsgpydh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vkzpzoaa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cblvmezr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zfwlfrsy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hybpcxyt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2moqctyyz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xvpsqnpi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmcsjnk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmbbdrzi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ldvpaqza.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fdwnxzct.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pripgltd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2axptbxfk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2simzgqyz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dhlpswut.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sgrfglbh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzvtchsh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2reqvduiy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lyvimgnx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2clvxueaq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fhodfekf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kxsckvzp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2riwoomqv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2azwvqitk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qzbqugac.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ftdbujlo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bzkswatr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2henoeqzg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aizawfgb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hrukdqhy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2snbaayik.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ayijcprk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wucdcbbv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2npjzwvxa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwmfqle.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2shpifnlm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fkeaynop.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bgcymatw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ibfidwya.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2egbgpxrz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xttaprgc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2umunlqee.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rwehzcuf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2drmywhya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccxsffou.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnjrqbry.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fmbmhsiu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pglcufxf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ewuegodr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2puqbzjjx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2exgoutwi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ecsxcgxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2djoiaaqw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vinnpexf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2cxdvivop.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yijvvzuu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ahtznomj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qqklatpo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2olxzihad.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kbuyyllz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jbqrqkss.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2upaarome.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cszregsl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2duakfdvj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tjktmvss.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ihdonyun.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fiusuoft.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnfvszb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2csnptvvv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qhvwdnny.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mfldqhwh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tkuxcukc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2abdskjxk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lsooyjdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nsnpvbgt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2usvqvvtk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2usutrxjw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2snwnshnd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ljmpbfmh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2auamyqgg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zivutnui.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2awmhnuri.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibumikvo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2clrmhghl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gujesbuy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ykzwphwp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zxaeaybn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nuskbwiv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pfuxmzpq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2trygxgqm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kygblmir.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2alazlubv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2olpyzsnq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lntarkqt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgdzsytz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ksqlhdwq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ypbjnfam.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ngjyjbtr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cusjytis.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2esxxubtc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wwujojtw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kwbucyul.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2auzsitrh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2oqukkapa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xddtowuf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2muzwroct.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vwertclb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uyplsppk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gobobzsb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wisouwew.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ecyysymj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulmuhhoh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ybkkcmkw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ppngijnj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jwzgvvqf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uyhccpoe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qoyvedre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qoznbqaw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rkxxwhrk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qmjmkgch.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ublrodkv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iexpdqar.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jpeduhlo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2apdbieit.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnuegxcp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mzfagiep.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qjraenfl.html


<!-- 参考信息 -->