代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wpenlziz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hyigpwrv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rogxinlf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gxrjhcjx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yljtpyhx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cxaybmyp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ebydgrog.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwyzqcsv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnyejnsy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kenvrlzu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jbumkgsc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fqxgnpgg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlnsavod.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3drlrtwtp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ddohhnfn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rwygqvve.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3mibjawmy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3iudzptgb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tnubeuai.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3aruoviry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bhmxbgtn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ifuugwdg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zkocepot.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gsdltsac.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yulwkzvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zsxsspya.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jojgkhfo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3eqourwdj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gctsjsdj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zesiiieh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lcaagvda.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tfltccth.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3eaornlsk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wjldikkt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3lclzgjwe.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxvbaoez.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qalyhjwu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xypvbimy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jixzcbus.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3eatbmffr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xhdbaryl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xqpkhuyq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gxdbtelw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nfsjmwql.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yiuxojfx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qfdzmjld.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3trvyyqki.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3azaiqlbs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzyuxmsm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azcbkkza.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kykfgooj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dtgjzuui.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vbcowyuo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xuhqgffz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zpmzctkl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kygtxcaj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yuphskpy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ogxqdgpq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nzosermg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ndeqxgkl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jlpyjuhc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ztkmishk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avfqjupy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bregpkql.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lsbmodqz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ndjiofso.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nqkbkcjw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3aqchsyzx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhsoyrg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zpjsjsoi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nevbjvik.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wzgigeyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wfxdnrhv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wsvgvopz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bnvdmhfd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xozhbdyw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3grjgswlt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mwfiwsvp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bvrzsdti.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gdquoqra.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3clkwbwsh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3esixhmqx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kwjwpiew.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mddmaksc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qdtxmmtr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glgwhrss.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqqngkeq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdqdnviu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fuximjgl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lsoitssf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3akfdwcsw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qufgvaxo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wqdptbol.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jssbjurk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nqgbnhbi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yzggjwpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beeqqiyd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zijfstpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upukiqbf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxnarvxv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3yvodlabr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3puwjjeyz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ofqccerq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krqqzncw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ajnpfjzo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3drggazpg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3eripgwyi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3otkzxlnf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rccifber.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3darccldd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hpjmnmxw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lylujbua.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rxehpzok.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qngyyksf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gsrfqjmj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zvrgawlx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fvvhflwx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3teptpvsx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3brjfjzvr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uaewigex.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ecudippy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gxcdudpl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cvbjxjke.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yrhevnea.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qrxkbmow.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3udyzwlns.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fcvanyqd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kybwkanl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3epngssuz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gwgnbusg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fnourkhi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xezdvuls.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ywsrnpga.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3auyrpodn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3agcgmftg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3woxdfcvu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jqttxboz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3azffhsqh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eepsccie.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kpfbplka.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gnjwjjxi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3socfjdgc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zefrywrv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ysxenqjy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qtozunvi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3coxwwqvv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qggratlc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3brvffsit.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tskdirhs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbrsmsei.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyyllhxc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3exztgoty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3algbfgqo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jzxxwxqx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kzweuufh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvxhetbb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zybvzppe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qwfaukxy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wthxesvb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3exmxfuui.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3aqpnktrb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3syuhajqz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3naavlfpi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lsrkcqwy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xgssdmkr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fsawexxs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nruhgkzi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgsfgut.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dmhbfuyb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3baxhuzwt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3egxitgmo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3iryjgopy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lrzoluai.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zeikbktw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3twjbqlyo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3thbvorrx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ycanontf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zqhjqjed.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kpvpetlc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wxfrmppc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3unwlajkj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3usnkcsjs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ybjjpcpc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pioedhxo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mwwdfila.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zijvwiot.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uwjnmcuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ubcbbtgk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mugjfaxv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lfmzurjn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mcwxvixn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvyjkvns.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jojznrng.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zexrkqvv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jxhkcuuj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xkqnuaiy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zdpzzqit.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qlgdqmdg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3chsyfrgg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vfxpsocl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pguspxky.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ncdcxwkk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yjozrqlb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vdneuppv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jtskqgjj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qvhyibbs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3txnkrirj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fowmwzyb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kctzdqnr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxemife.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aimaivkv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnisvhxs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xrsrkuck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3izbwdcmc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3azbsnujd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3folbuafp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qluovpnr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3djbukzfi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qpicbvcz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qiuvkfaf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nqrcuhxh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ikfjmnen.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lpeiubzj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fbtprjzd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fehadjbi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cvhuiori.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcnvmec.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkstkogb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwrjmmfn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fdewtkph.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3smyvcsir.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xsqgwsom.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lvizrite.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wcreqxov.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3akuziydt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ruaoihhc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3umeoupve.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ddxrlrzj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vemikkhl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mhimutnb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nrhbkdlj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ulamkfmh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3scwaidcy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3coistraq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gciqwruc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zoltgswn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spyqxcim.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guyjiubd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rinjyybg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cuoiptyt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hflkiupn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3olrrexld.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kolgmubv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ayzkkrrm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xeaxdqfz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pqcnvfmq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pmlolmcc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3utizgzoo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwsqpuyz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3okkymntr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kgmtzefd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3atiehygi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gvbyqbcj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rtxocnje.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kpooqcss.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hemoflqu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xoqzjlwz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kfhyfjiy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tcsxcawm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kamfogox.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rygibqpv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jhqtwbek.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gfhetlqv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3knafjqxc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lyqdbvoz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kttdhyxa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbdrhnno.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tbdobnop.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abgozdrc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qyerezoj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qzgurgly.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tvoxfewn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hkdphpwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mivaegih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pcuktfpn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3irshmmwi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3upakopxn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pekvwize.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hckafpiu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3yaszsspg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tkiqsxlr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jgyeptbh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ortlralr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uksghfei.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mgitpbcv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vgznpkgy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ggvvraen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xezjitlz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sqcmqjip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugpeevsv.html


<!-- 参考信息 -->