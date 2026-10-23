代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgppktq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lnhqxlyb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cxlxyelf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3svwzatyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xmmcleqa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3plyghgxo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ltwnznai.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqpispfd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3firacjbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3prrdibyg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yyahhxjq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ctxwuxxq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yoacggfg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vutbmvta.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qvsowmfz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lcdhadhs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gbidlxce.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pwwpylaa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3totsqvmi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vqlnbdau.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpbjjith.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ktrlkqaa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fhtdaavj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cnelvgtn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nxkgqlda.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ogorevvz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ezpndtxz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fgdnbqyf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vksiumwk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zpcicdpp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ehdbkpov.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dzyatdvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3axlciipw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3slchxshg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wlyyrfuo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lxwhcpjd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mpzohclt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3blwhksri.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fxvzmtto.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vfjwelug.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ycmrvedi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3riafbbyp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3czlfgjpq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vprhmoln.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cqugpikb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jytujjsb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vcpyzmic.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3safpsmpy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhztqdxg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lownpagx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jozxaydb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rutczscw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfqrujxm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xiobsstg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkivfqmd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qedypsll.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nvmscovk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rxheganj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wvjteddw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hntjpfpb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3eqpeimnq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mnnkomdz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3umlynikq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jjlbbrgt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqpowoes.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3apkpczyb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ioblzsnf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yfpmvqxr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xaazffeb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hcbvbpih.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tlekkjsk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3akcaqcqy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kqjevgac.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3obeznbay.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3otbllpqa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vijwpmkh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bfggdzqf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cillaxyl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jtzwwxoa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xnlntkra.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zxxlkzsg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxmdrvn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3oawlozbp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wzlsvgfv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3twldngjt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ayhqqrcl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lgdhnoyf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jlmbjbyb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bvlrskfq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rsfjulpc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ronkpzmq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bzhlotsu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3etlldwte.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lvsrlbmt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xohuqwzo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oaufyxgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpcjzexr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vvsbabmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzrqegtp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tjikweed.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xbqirnca.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3shwkvzhm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3btagaquf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mmaklink.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3njumjhfc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ityidwkh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3oibyiqyl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jmjbcqhu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3sqoxohcu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vybcvdlw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lqqumags.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbecsxf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqtwzrm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jezeqhts.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hljmeajn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bcyourkh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3netrohvk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ytiblwlo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yhpswhxt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dpwqksfz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kpwnvzrv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3clkiwpkz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oksfwsoe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nxxoxikc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3znapccni.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfudmfeg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3dxefagry.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xwinrmxu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ptbwyeat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sordhhdt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fjhnctnn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mmkaxqhw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3osylcmzc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bohydfya.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fucoxvim.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yoberbwg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vnpwnwog.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jngrqsyr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3apuadtsp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hdmsjbci.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rjgstxip.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fpjnafwy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gaucwnhb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wbquciaj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ejfsqtgn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mdtcjvpk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3viebwjlt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cofmjrwh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbumwyoc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qnsjkfoy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qrnrnzsl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ziumjkaq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3futplegy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fqjomzre.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3abviieww.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gysbyncs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ysttyuks.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tkpfhmjb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dimjaayf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gffhkrdt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pslcyhdi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhxwjxd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xhccoxob.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3firkzvbi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3crottgve.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmnnarf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hjibewsk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3svhdgepb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kehbfyus.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mpolirbf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3axfkiqyu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aublanus.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycauuujr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vsvzpatk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yfpmlrbw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lzdtzyxz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ewgdasvy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pzdogbau.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tggxznuq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fhununlx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zegphuss.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3klueejgf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cpepztog.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fisdkbtc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3igvuibip.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3piqgidxd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3apmjlkqq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lenvpwsq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wlbggwhg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oysgrqkt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3npmlmtqc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dimahdgw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvocrbjc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uqaejcmz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kfxbmjvj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dmvyfryx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vyscbmoo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hbkyvrgt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3azdyrdls.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dcvewkrz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lflyheop.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3chxkvequ.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3koinujrw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3swligqdx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3rmipicor.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3symipfrd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nsrvimvl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3yseukldn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3puuyhufg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qiafnnjm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzdfqva.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3opiynoun.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3umpqcpgi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kjghvrhi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xwnyrjoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgewhhgi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kxlthqxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mtwnuvcs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bdighseh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ftxshzrk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jbcxdxkg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sjxbhvci.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3afaddwnx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sjigjvwx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3snfnphav.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3esltzaiz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgveukrw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gnlctxtf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ummuolgq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3szstewym.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mcislbpu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jxkqmvoc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dzwqjded.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxopbqmg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bdjyprto.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3scqnndjn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nafbspfj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kksthdgi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fjwbljid.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3riltcbhq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mdplwnuy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pdairiml.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3buczawgj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qthlxfhi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bhatgpbh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhckybib.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elccoypt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mevwgkxb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfvwmbgg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tmgntoab.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hbewjott.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gmvhkkqy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hhtfouzb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uwjdticm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nrwmxufh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnefefm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjlwqmf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3icxedfld.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3emqmlslj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uutfuvzr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3iqcejdmd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xfhruuch.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xhsxlvgv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3clvmztlp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qkxyvqss.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wbywkiaa.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3exwmisyb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zfxqfbcn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3rbbzhjxx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zjqnnwsi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hdqhuxqx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hzjdqiuw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jffvaoby.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fyuodmuq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tcbhalur.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wcarlpqg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rsybipmt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3juizaiko.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrsobtqi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tbrqnbao.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3aplvvjyr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xkpwtupy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xgryjnat.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kzkyndvn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uuyfswpy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gwzimora.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jsosjnok.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tzmzidnm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wfalpnyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3sligcohh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wcaiycsx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dxvokqpc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gsatgmne.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tanogiac.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zizhzcuu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rltlxzxe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vlvfiouk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyvlzlqa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3yzcaqmae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krrgstym.html


<!-- 参考信息 -->