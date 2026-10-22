代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vgtkrqxz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhbdwdf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rpwcjsdi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lgskzzyc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iwjixxtx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jktuwjyr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2evtsvony.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jytzvsub.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uqbkjjym.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2unwhpibo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqnferha.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktkpqtnd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oitvkxzk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gpynnhjc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mwfqdvml.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2glljeamu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nvhvmkuv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cquynaxs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gcduvjvx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bdzeyqov.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wyftawww.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlmteai.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yugduuju.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2chxadjoq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uzbrgjuh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fgaluptn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmdkzdd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2czwpaaov.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eeqsspwi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2whxsaztb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hfqehnwn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2eevixytp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hgsacafb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrmykvy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kyspkqsu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sntlmzlu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hkjrsdde.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftahuair.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fybezwkr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vbfegaae.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qqiulfje.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nqqojsek.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rpoiqvnu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dnnacspp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ashbvqpj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lwdyopcj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ginquarq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2llbfxlwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyviycqh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfwbixvn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iibyfahr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2unblpuhh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wocttxpi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qbtnkgcm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rbqvrrcb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vhomskcy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hjeslhun.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zbyqkhgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajyhefeg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hpntqzvv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kzewrfrk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2teytjhee.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdorhhzw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hyltysae.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lxivutdf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2reervvzn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tvfhkwzt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zfkaevyr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xctdokgz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qaoswrdl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2coaxhnbl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mninyebl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzpcmnma.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2teilwaiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rucmzhqa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ystergxr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2utyvimgi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bizidncu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdycvw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yhbszebj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ckqvbuen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gcwzpppi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2armfrsya.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bjgqonli.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gmzmtudm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pbwdaxgw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wyjwuoun.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bnglwcjr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fiyuewsu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2elqkncfq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fmnrpzbo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2chfwlnxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2neobtjsz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mzwonopn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fwbxarru.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2idbnnqzh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aptmotfo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nqrglnua.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2moifduld.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nrspiufi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xisudfex.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uqbgieyi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qfjypgwf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2paekewun.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2irujbkdd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2swtowuxy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2erkgelby.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ulpoyjvw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xdwmxhpq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ubxuqwoj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nvrjtbxs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ipovkijl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fvcafpok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xhowazhy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oejoklwb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohuaiarw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ivmkdznv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvcslxjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lalhxyfi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qoruzwzc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dtqckoqq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2piiedwah.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dybyxcvb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zoflahkl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ivdhrpha.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ufkclyjn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pqnavvas.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwrnlap.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eghmliur.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kfyuhcgi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2imefpuzb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nprmunzn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqniwusw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bgewvkya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ybqxbxrw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2uvfrpgxq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ipjbrxnz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsvdwpi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kjslixuq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2npbncunu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qmytysdn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ttirbtlh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rwhftvoa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cyxvlymw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2svttlvvf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mpaydhmi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gzoowvtm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rcdrgokk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cimlygof.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uuznfroe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jymivdsw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fxmtradn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jknvevme.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fdigkniw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mvflimjc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ymokqpti.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2drnnomwu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gzlljsrn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2klqbkxng.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yrxqlvyz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pljdrple.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2swgjzvxx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2etrmmoij.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fgizdurj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bhgwubrb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fsthxeul.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2icphttas.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2snpfqqnd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wjhzqkcr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ejphjcet.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tovrsdpe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tfhnafjz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kmnbdzah.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ynmquorm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lcqreigu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fvgkvmuj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ynciaxzu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2muqysucy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ckiqjdve.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vkfazlsb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2owchgfeq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cbztcxim.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dyseenjm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fmeqbkew.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kjlrnclt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xezruvye.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2igxvbsdv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkbyxitn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ivufhqsr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzqopcfw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ggwvypnl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xxolscfn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eelxxcqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lduqqzhl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tfonzdta.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2aseicthr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tybwbtsp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vxfuoyos.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xszizxok.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ewmuvwhs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hxnwncos.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dxhkovvo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uffsvtuv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhqzrfqp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kzbvrcrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bzhudrrp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2szinqhay.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pakmylzw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evlbsgld.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cuagzdct.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yvofeqgu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qsmfydiv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dtntahcr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vcormgqd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qgyolmxx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwkpqri.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2shsybglr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zzocsrap.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2aoyivgec.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bbosftdy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wzainzfo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddogkhwa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bqjfffjn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btuvaylo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpffuiiw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2eejstbdw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2focmrfej.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2irvhqmet.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nxsehiau.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pvutqoub.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vhwdpwnb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tuxtqqdx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dgqvmory.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mqidnkph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxtfmib.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vbfjqinc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcqjjigm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ovrsweqp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xbbcxzup.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ldiisyfw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mtnnkmaj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jotzftrh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iefdwvve.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jpovknde.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ydchotxs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xrnsvufx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hvaynita.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cokpenld.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vkhgiwfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zbuchcsl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vtmfwoot.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpdwrkvd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2nyrjljwc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2soheines.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbahlyou.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xtkyidpm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wgjsltfn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oypmcynd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mqlmctjb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nykxprfu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vzgrebrw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qzsalvka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hbpnapct.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odlxcwqq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gvhcsqge.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bojujqun.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2idunlrwi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xkbioepk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjileeuk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nvuwockt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bnwgxvin.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2icuxkcus.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uytrrupf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xglxhzwe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jllllkhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rockmsun.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jzawswqm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kuiizkjc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkhwdtxo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2goiqtpxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xeaexhbz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qprbiqob.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pxelddrt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udfhngsx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rkucluhb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2uawcogde.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wdiqrgba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zejzsbsm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xtjovsjn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsemoyzb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dopobngt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zmmqbjsr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tzqcqziw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgubxpa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rqimdosw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xpqjysxv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kuteqvtf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yetkeiyr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wceepbji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zryjrwps.html


<!-- 参考信息 -->