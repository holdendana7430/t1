代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oekwsqlc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltvunalk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nngnkkan.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwrgvqrq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3drwckgye.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zkmsrtco.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lkshjdfo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3eleybopy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zlrxwdqp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hjslzdsy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3heidblyw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vvasttol.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yyfckxcf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xfxtdaqu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwivgt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zdgpbjeh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cpmoulwb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kuwkvzel.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ovaaovhf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3exwnqcnt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bmnadxzj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3doexlxrv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lhmnpruu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aakwbotk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3carvwfjb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3roarkzsu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xwsxkpng.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3usegtnat.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ydyrvito.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpjxger.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uqhnetxe.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jmdjgisw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxzmjea.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ruquapov.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dajqvimf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3aykbhxuo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fjppuvud.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3scjwsenh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gqrjitmk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jjtdyxlc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uqwxyvqi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tclwbaap.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ofdeahqy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oshuoxfo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxopoz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wpeniszl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rrjyvwfa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sauxcmtj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rrtvxxke.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rpzapyhn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ivgqcqpt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtrylthg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jmxondpf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3psgadpfp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3egjhqouz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3csdrxabm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3enjbexta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rrmnstza.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ffertwyi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qncyxwjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3assbourh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xtkscscw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tcwkirdl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ndddravt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3svkkafhc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3rnnjgrpn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wdxxtdka.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jhegqnwe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ocvckgcn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nuxokrlu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kwesmphx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3crdhffta.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oduoenwu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nutrwkel.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mwgpbwdr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jaziaeoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyuanegj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mbybrbjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayosrdgg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pfwwtcgm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ygerbxxx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lykltxou.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3erfnwioj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aopjytgm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oxbqkriz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sukdujjb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3sksuzkhc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iarubznt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dlqkztko.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3amqblnom.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wogppond.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kwsdhahq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmombsz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohnzmjtf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gjetxowm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ejrbcyew.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dmrltphv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gnnwxkxh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ebvurtmo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vivtdhir.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgivleh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fkohjyrw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mxwqgcgw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kjwlxint.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hvqzilbv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhsrqkd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bpfwruzm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3giqfqzev.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fznujudk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mcvarzcl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uegvbvke.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uqseapyy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xtaryakf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mvcpvqji.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3groyywlm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wmlyfzrt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rdqvwgss.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jewkojjz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmuxnckv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gvknahhg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3etckywen.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3faueqqbv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3egwttxsh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wssqgris.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bsxtboqs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jwerkmdu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mwtcvrvs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvcvfdkd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbgwjnwp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lcysnupm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nmyymgyy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pdznhnkv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bwtpylvs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ecmjrkgj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3blfoehoa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfytfanf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nelxvdgw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nuxicigh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hozntsbd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrxkwlk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wluygbtv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hyjjuuyq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nnypxtqw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3alygnvgj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cktnbylt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sjavquwe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uvyjdjle.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qgztusiq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3afusltzz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xfpxljfj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mavmkvwo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xuzmzomz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kkxvkoag.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ctabdsfw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qkaibruf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lwceawey.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhzwzlvd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lzcehfma.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3civrhmob.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yryvuyir.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rpedpgww.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mvttvwbq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vqeeyaaf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kwabnysn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3brshprfq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sjuekmof.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3preyxwcf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prohbljg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qhokbenm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3szhxuygj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sxwhgyvj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ovjelpav.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvzzaksi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qkvqikuo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mftvcten.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dqungvxh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gjgwvnut.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3atmwabyw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zmuqbqrv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dbdqmoho.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ppldrcei.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bydigxqk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aeawabuk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zuosjjtb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3uekbednh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mymocymk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dvodhiqh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hnvkmprr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lauxlqym.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqbmei.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnagfavn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kexwrbsv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3surgilhd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sutblbdh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rfkvdedw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3glabljlq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ejjlnram.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nvznvnti.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ockkdbvb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gxztamll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kebqfewx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3isgfmazc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xyxeuwef.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qcpmiyjz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ltubfzsw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yxlttmte.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lduratlf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uqcygyih.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vnrielen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ljdhlyhd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ugtfltna.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uddxqtta.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zelcvkft.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhonsnb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xwljjduh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wpkedxga.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jxmaqhxf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3exdkkktt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vueokjbg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsdlibb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ueliyhrf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nbfnpyed.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3labiavha.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3anrskqpb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lrzqtqpg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ivdketho.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jovtuilp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hspnqzft.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3perabdkg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3plzewpfv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jljkhiau.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3llxynqkg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3idowtqre.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3eiupnddu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lmcprpjk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aoolbygf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nbwvrtyg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3avdggwnl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lputmgml.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mfibohpr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxmkycez.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gozlmfzg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3boawqudo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mimgepje.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbqwyacq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wqxcerux.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzgrnwmq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ivejviml.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3eaekimst.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dfmaxsla.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3joeucxuj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3limfgihe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3temljbvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ilpibpkn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nswpmjia.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhuippfd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjsgjrpl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wetzwnld.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpvxgves.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3dccdyegm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ahfhmvfw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3klphvoha.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3csskoxlh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xdpotxmy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hbwnixho.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pvlporlc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hfjcplzl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zdhfjjno.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3axpgpbih.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bevupaof.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrmhrjqq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iulvtcse.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dstgcsgq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jobjnxjf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3azcgpfzb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eycjxbiq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yakwqbgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuztzmuv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hnukjlwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygmcpahv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaerqjei.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mojsafwr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mgwrsbch.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pxmvxser.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pjrjfmby.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wqdxcijy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xkwovlxd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgkzgpeg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ktfivrgf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdshazzg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gorybpza.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lmvqipoy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3weuthcxn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aicfwnsu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3eornydvi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnwearp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zrorqoqo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebmeulnw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kpxaenvp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ppoliazq.html


<!-- 参考信息 -->