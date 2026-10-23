代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zivnizso.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pgeiazap.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rxphgiyf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcuzowyk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3raufmoev.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3efcgglnt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vtduvhkk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mamcwhov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snubbwbd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qprxkgog.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3swadolsp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nvewiqha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vgvirmva.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tbydtppo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oqmsgkzw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bzgouhhk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ympzsibf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3epbtfmom.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tfuxdtuh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jbemfgvz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3isgsjzie.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uipjurbs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lyyccvqv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wtxtwrrn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sufajhba.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qvcdhskb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aazntwgg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3egffoyoj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ytzekjsz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pwslqdeb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbzhzul.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3idlgvowu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ujscbehm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3chcnltky.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bousfsih.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fqczfrub.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fluvrgmn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ojxxircf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3prbojdta.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vclotduw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qcfxrmzt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mosjektc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gynaoxow.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vxdubtlo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3glrvhhbf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npkyumsa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrvgqhd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zupfuldt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ctcnwnjz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cynsoehg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhtojesy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hrrcfgfv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qqkrbarp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bmhjezjh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3htudsift.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3assgneqo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vxjdcxch.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqxzezwa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sqwsjshw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnmxajr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3chctaink.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zyxprwxw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yslqalxn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ikcnlddo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ycbuarex.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xffehxeq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jnsmcnla.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gfjzrngy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qyppefel.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uanliidu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gxjxawgd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3htwapyxc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tcglazbo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mjyegcty.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hfzoctzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vuxeqweo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hysezafa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eamxnxam.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dqywvrqu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3prrtkdte.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vfkakgla.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrkbrqi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dekpuhqa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rmvqkhbp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hpqxwqyi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nxufpuls.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wexxmihq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3urltntxl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uibqyqmb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ayawigsp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3flzxxrgz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rzktktek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjffjbgd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xlnqwxik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shjnyxag.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmmasgdr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uwooiqmz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ripcbgxq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pevmqtjk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3smholvys.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sndvjxgw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fzsumjcn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kdcepivp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvhiqvla.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fquwknvs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gsqntcit.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpeyhbom.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dwfzrbkv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3snkyyzte.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3brzypvuh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vwpzuupz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gzkaeeox.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wsvpgegu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3icdeorrs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aacsmzvs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jjwiactp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rxreqhdt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tveiigbz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vohwjued.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3voaximgr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3iklvwjrt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrtgwrm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3byzbwkwl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nguuinzn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3gblfilae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zclwplqg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ytbpsicx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vmqhvabo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3pmczvfaa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3klepmnds.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vxekmacv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3offtmgxn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gjtkrhih.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3esxmhnid.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dkcvvrwj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3daixqqjr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wvaupmme.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ksudtrio.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ltuytgir.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rpnnvret.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wwbemyot.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yfbckmgc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xnkktzby.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kiaxybpg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ucvlllfk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jcfjuthk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ogxwpbsb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dyolfqau.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zlljmkis.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gxaddncp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lvjjsoqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvzzhkow.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jpyoinzg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aibxpcjd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pjwrnjrv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xlazdgbq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3llxpgfpl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dppvreke.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tbecrrqh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpvnnks.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xtccaaiv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gdhdwuyq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3munwzkhx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3puhycicv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3feyrkvss.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pjhszdby.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ouimbnpw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mmqasrqv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksacfcsd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwaxvlob.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jijjpvje.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kkksvpax.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ccqipkyz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nesxoccs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mrlxjhds.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3htbewcme.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qdnylmyg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3obtwrmto.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3aaumzdkj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tyfesoll.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ktlqurin.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3scudbqns.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gckoopcu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bcefliiw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3exggmkpx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tljkjncr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wyctdujm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lfvxpivb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cpffdimy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xjkygagg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fnrooyew.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kggfjbmw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jpffqgtc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sjyunakd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jcsmafam.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hreqrgsr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wxmxouqg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzhgmqez.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cebhmerd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3venvymtn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mffwibqg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qlbeaqok.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qxzyviot.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3htwqrhvc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bxsbpbfs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qapffloi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zexkjymn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fhetinah.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3btlplnhc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjahpevo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xsvihuzy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sajnpjsb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgguea.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tqwnokrn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jmzfvnsy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vywntnmz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ijzwrsys.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tdezslmq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3harghazg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tlmddqhf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyhvpni.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3stryjsoy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yzjeypcm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nsckelbe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdnbhtn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xqrehhde.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bnzwaeet.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfqzkafh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qbakoksc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ozqqcrli.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gfiimcyx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3njxfmoku.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wsgwyujn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zvbommea.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3njbfcnvr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vkupputd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dwessyvp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uzchxjyp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3frdfxenu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3keseupyj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fcolqhuv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3itopglbp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tekdwijt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uklhkuhe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jgzipolv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qaizrsut.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3grbnxjbx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3njwfxand.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3aszqyeko.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kkxbniyu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kdbggmtf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3inacbnuy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gslvwetz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxartarq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtkwhea.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fqmpdrlg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3annxvahd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3guwavjpr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rrwyznpi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qvzcnuqh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3icezxxth.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wizocszg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kpihikgn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tucbxmcf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mnxvtmak.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3axxdbvcj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gfpcjkig.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ofjixiuk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cdpseulj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdvfdtkb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jdnlhnqo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiielcyx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyxujxmf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pzujwlra.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yilaxrlq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3mkgnritr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3utwqvbzn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fdkricyb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nhkytodj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kcqqzdbv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aefiayzl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3otipesxk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eouycxnv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fnoxsfaf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jqhitqpv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edctqkcf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pczdrbus.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3esruifik.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wkfrswhj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hnixvtsx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jpncrfdx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hijktjee.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wjrdaukr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqcramlz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ceibynug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bktdyybi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjjigsxj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mtsfgkaq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzfxdsyc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wrnrlnly.html


<!-- 参考信息 -->