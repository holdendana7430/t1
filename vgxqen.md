代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cceblilo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3znviqazi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hixzudpk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gisvtfzx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tzatzmoa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aswmpqzx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enemjnew.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3osevuuai.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yaylifau.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lncvvpuv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mvzixnez.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3czwruusd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3epvlngka.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtotxuq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kkoqqwxz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcgwexmw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hvfjufra.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pobvizkp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxiwwzdl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pgppsyja.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ysrfekpm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3slfzcrbl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lxkubgiv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qpxtvfzg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3akcuhflz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvymjjc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzlbhjn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3budrwpfi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3aywqycan.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3auhzzivu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zbqwpytv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3magwuemm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wirekvbz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xhogjwpq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3adpxfbmq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lrhmoipm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fgkuetfi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fegmekkq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3elugdoju.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sqfrmyfn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xaibeqhc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vfaruhwj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3idwlkdza.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftxvthje.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fikwiiwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3utdacggb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bckcztrh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ybfnwxvu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vchjxpck.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kfequgml.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ohjqgikj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3npzxucnj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3blbkdrgp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3amqnmbov.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yoisfphp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pssmusoj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjpieoku.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fkdsfcds.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnghamt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3sftmfepk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhrlbzzf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3munbtvod.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3apzqjtma.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rwurvspk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rcyrpskr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhwmukk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fedhgezh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxyqleh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sgykbeod.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cxirefip.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xclttloj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qwfucodn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oyefmryx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lusiwnef.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3egpfocnd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kphkomjq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tsvchpim.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jgbikzvi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xdurmqip.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qgbmrtyt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nausfxyg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tfagxeuz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oagrwsoj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ureirsjj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uxqbsmut.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uixgszog.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qmzpyqvt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ekizojvq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rfyswpfb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgnvbhz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dkheqgqb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgaoaexy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3aocepoxa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cetmogpk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nfggjdiw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3phpgevio.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aqeekxom.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cryvsaet.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yplgzzft.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vtbhqgcp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xmdeimzt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lpzktvxd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3drbsxdgl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmrjweb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cczumyea.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gljalpju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibhqsmvs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rgussvtm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hihifyli.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3etfowhie.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hobspfxp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jqipzzas.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hrjkvidh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jbalswvb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rlyqunbt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3szrdqagr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fgsbmhct.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3osfcguxj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3eciiggfj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbntpfc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nnpzvtka.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdqpnqaz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvmpguu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fivrxuzp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yechhxtk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vtgxdhmr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vlbhgazo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tnulvkdi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xlsxalmv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3adjbmjps.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vjnfxuvg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ecdsmopy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3uonsapwl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vygqcpfv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zzjogffc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ggrbdxjf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rracbcwy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jusmxlby.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hagtmfcw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gwqpiiqc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wfsydtxr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vbcefoxf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gjvyyccn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3urgdlhta.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3yhgzhlhp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fydnvhdj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jypwhwjc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3etuabmtf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pjyylusp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lhzvmnoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3akaortlr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jtnbsshd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ttqunpjv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iytvcgzm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wrhhheai.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvetbncv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nilluphj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wxnvvryy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sdkdtkpy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3riwjmwzp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nptnjjgg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iqaevvbd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kphdaejy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iidexuie.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3upkjegio.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3iopywdhi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3obuypjlh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzcfdwdk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wqfhilav.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3taryydpt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kfilwopl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lngmqcop.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ryzmqhyw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mjmhsvoh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qguepnty.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gglxzdki.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kamqzmyk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3heaecmhq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kauricgp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xsajwdzv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzxouud.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uuwbqttk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrbkshc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gzmkuwcq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gidbplva.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uhoobsiv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wfhsvvns.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ddvylxbq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3htypussi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3trufayon.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hfnyxmpg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3faojmvfq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3slsscjuw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3afbtilnw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fcajygam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pqcecizy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ubecarmw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ffhnndoy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bfhsyuuy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cyrsxyfs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3klmmidxb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mpltfcoj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3afzckblx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ijlultiq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xiinqeqv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uyuggbxc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dtlgbnto.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tdppthmd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fzyvdwqa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vlgxotzg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qthkgnjo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qgxzmxqr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ledwvfyb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ukbuhcem.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vjropfmm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wqdouhcm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnsqvcf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkonpyyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nifxofaq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndaeedjz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoujvvhw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uepnrfjn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zlonaqmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3imnpanls.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tsgacjvm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kfqnmbty.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dcysybwk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vcsotqxp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyvbzrt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gdghptkg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gbvryapl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3erhcpcnd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ioabnrec.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xaehsmnj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ukjlnnvg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3psskzhwd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frqontjj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bzbjlpvq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3czhjxkby.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjrorsxp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jotyycny.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mkdgpblz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lchtyond.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3elhjlyjk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ckseuqey.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkanfmm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3isaczwiw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mkiehedb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3iewincxf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wxhuzogq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3depewaqj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vtgdhiiw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yenbpcbr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xtbjvyzx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vawvtxtc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjhkbzn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ettbrmiq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3febootru.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jvxewkiu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vahfsngc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kypuwsxf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3onrdzyyh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nskczejy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxrtoac.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vwbalbqx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3grfwpolm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjpsple.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3asmcxauh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmhqefwn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zvsrwini.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wnpkocso.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhdlhowg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fyckqtha.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tcbtteeb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ibwywwju.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dmjypaui.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nejnrute.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qlaxnjzq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ilyjwedn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nvtgjzxc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zpnuvqhu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dnqqnput.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ajkqkvyv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uuzqoxbs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3eclbnvga.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zfbxqzxj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jhhhagwe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kplekuyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wvhmfsmf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nclzsbmf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xewjvdbx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rulgzwfb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3syccxwqh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3oedtepde.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hognhscw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mhlfapns.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wfenejox.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twsyjrwj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xflmjfpq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gtjeywbb.html


<!-- 参考信息 -->