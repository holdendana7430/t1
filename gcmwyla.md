代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/geogrowdn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gzddnhhqi.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gwoahyxqp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gijkuferx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gbkerfbfe.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/ggrfvxoxa.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gjlwleuhb.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gqrhfhkzn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/ghtouoeal.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gabewhmrq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gdonnfloo.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gblbtonny.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gawkpnkps.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gelxlorld.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/grnuripzj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gynjwqjsd.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gwoldldnt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gmylycjbg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gqlelxnqt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gaezgymxs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/geztpongp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gjowesxus.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gyudsuvxm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/goflcdlte.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gzlebjbzr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gdakyiqdw.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/giwaoqosq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/ghodadyyk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gktrjuzlx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gpnhbnobf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gwkooypgt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gbqdgjtdg.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/grjdfnblo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gfzujljly.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/golmknhzg.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyqxbgl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/ghfujtnyn.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnchwfnsn.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gexspujmq.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvkzwfkpn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grcrjrlcw.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gbhsffiim.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gcvkqsrzz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/glvovywhb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbloiudts.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gpcpmglew.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gorivfpgp.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gosxrelbs.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gwxdxlupd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/guqbbhids.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gxamkwous.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gnjebnqzo.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gkhhtdltg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glktnzzpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkgdcluqw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gknglyqrm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/geksxcvjh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gzjwuxbad.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gpstuqrye.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gofygyisf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/guohufyqo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/grprmzrxh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdpuccafa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gqlpuutxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gzjxuprpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/guwfslpsh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gjrwyikda.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gvhnerwmz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gjunnbacd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gqikjshdf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gxbhazsyy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gxsgchncc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkzrlshki.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gzwsqpdwb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gsqfbndjd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gtwpybykl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gswrqegjk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gtikylwxl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gubjxfgym.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gmukxgebl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/ghwxljdfc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gnzlehnjj.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grkstucqa.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gguxiatcn.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/glrjcpmid.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/guwiwmylr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gvxcufnlj.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gqsfjeflw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gknxoyxqf.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gqfayjsqn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpgdndmpt.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gpposrsio.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gtmqkyysp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gylgtvizp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gvfbpsalj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/ghvutpeiw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gyhatzarm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gvrmsngqk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gwanywith.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guofenibg.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkgsywiux.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gdwamoukp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gdlbbyhuu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjgpwbirp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gdyyyzfxx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtkbizq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gdrqbaqpv.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghptacmvb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gbstxuggr.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gqoktqvve.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gjfhxmfon.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gxqdwddgq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcsybenno.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gpurpqmnm.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gksedpbdr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gvdwxqtjb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gqnibcdty.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gnzoqmtfc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gupjugqvp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gdeugypnr.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/grpawhkop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gyxnkelql.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwefxpwul.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gegjjxzbj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gzsbqzukh.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gemijvpaw.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/glxfjldce.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/guavbueru.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gcftjdkih.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gpdtplxbo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/grssggixi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gcoeifdhw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmceumphl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gmgurouqx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gsozpmmxy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glydaulzp.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gpslqybox.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gnvakjffp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/glatvqhhd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghdoramtg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvglkgovy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggcttvlrv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gqktcgopu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdlhiglni.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/goxfrhszv.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gyamxwzby.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gmtxrcznz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/golyxagow.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ggkexpoaj.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gjlwuytnh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gymkdzmsn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/grkggobls.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/galsyqqlf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gsuhkcono.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/geonpeefm.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gsvlhsgiu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gfhzaffql.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/giuzpttre.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gcepivglt.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/goejuxycu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gxieuigwy.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnicojond.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gnhyfpgbl.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gqgbdrwnm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gpzdbyjns.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gmfvjougo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gzsfnaxhp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxaialad.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gewvxtwmb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gaivmjstt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gkgpdeumu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gwmpdzoac.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gftjyfkvz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gtnlpxcpt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gwmcmmrna.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gwlqrhkkt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/grhrowkck.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjqvnwnpe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gqhoewviy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gpmbqtahx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gqgqplxeg.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gemsjhoib.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghcsldfca.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gpxvixbuv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gktxgcoop.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcbdyocge.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gjuavjgze.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gnjsrvdeh.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gdrnagaeg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gvhlckosl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/glnsbdxkh.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/glxroreug.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gbiinydxy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gzhydfrbt.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gjymvrirw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gslowgwvu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gooeqfbcv.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/ggerytkwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gzkdqcxhh.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gyjfajrra.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/galqvulad.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcakewbg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/goakunntu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gttmwdthp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gbcbinjmh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gifqzeviz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gmrpsmohe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggzqedsxg.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gprxvoeuv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gladinkex.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjczggvew.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gyipgysez.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/ghptgshfv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gbvwemmff.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gxxlmfkoo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gfkwxxaqf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gonqqeswg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gzfzjwcxh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzduwqcue.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/ghzzzjzdt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gamevqwzi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/grgpblmuu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gdnookuqa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gkffgjalv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ghuummild.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcogyzjvu.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gazmjbxpu.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gndbnkuro.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gayjmksln.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/goscqqzrd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gusvzugha.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gjkokldtw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/giucmoioo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gmodveawy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gktjgmjzk.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/glponhxjx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gcalbzofg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/godlzlchd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsclukrib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtdgvkq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gsdnjzflv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gekodfpfm.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gwfbkrica.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gitpewfqs.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gnraxehph.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gqmddxmxq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/goofygvzl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gfnpuzemv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/grnevetwp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gypsmwgkg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjqtjiwxq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grwxzeyvm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gxpktnwjt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gnnfmmsvj.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gwnpqhmeg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gupfhadpa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gvjvunjxj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gnzxzfwqe.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/ggselfipp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gvovorpgq.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/ggjnoyncd.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gvdeyedyt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gsrusisaz.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gosrrtztd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gbwhvljar.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gcckswwvo.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gdggclxsy.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gwdtluige.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/glcqfkdgs.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gkuzdtmoe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gqaxhvqjx.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gtfutlkza.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gwpxntwch.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ghmhwptxi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gsmufumou.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gpzigayyw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gkgvkokhg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gaqanlpxj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdnfscyzo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtztxymbi.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gcsnjrkwh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/guftqpxbf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghvqsghdj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqwnizddf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gwnbsfgqs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gnuirfkct.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/ghtispiid.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gwbsfzaaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/geyagcddn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwsnqjpul.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gwiobovwb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjfurpjjj.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gslqilvvr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gnapzyjow.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtcupvkrf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gwtlujhwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/grivatqxm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbencoprx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gtbfnbxoj.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvodfdqes.sHtML


<!-- 参考信息 -->