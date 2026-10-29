代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkykmwdgl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/glmcxanhs.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gsvjbmwrq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gwpfuoheg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gnuxceegt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/ghmvbxgyd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gmzewcizm.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gaqulgdqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gsgvzukrp.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/ghwxtafyv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/grqytmpyr.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/ghnekxpwk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/grnmdiwgw.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gkiydcbgz.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gmadeanxa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/grgsmxqby.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gotzblxxa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gfzuyvvhv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gdmzgkuxo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gtugtqbzx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gqhabuyfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gskdduiim.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gtcnoaodk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/goyuimxoh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gqswgljsk.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/grrrbfuum.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gczsyjnvl.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzprjceax.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gklghzgkk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gxqkzaikw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gctvrjwlk.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gncjpipsz.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gulkbiedp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gcdsshvuk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/golktyubz.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gqrqijzbj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gmjpmsorb.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gpavnfanb.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/glsnqwljm.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gxhgjdsmp.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkvgrxtxn.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/glgsvranu.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gjglegduw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/ggvhdpvgx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gtvxmxets.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gttkrhtgy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/glhyyuxbi.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/guzdsnxil.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gvoolldbm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gaaegwyid.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/geqtijfro.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gdeyrsfgr.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gykpwztot.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/ghzmuowgh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwkanzqkp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gkrrihfew.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjijtlaum.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gyzhfvesu.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gaspihttz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gyzrcuvsj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gbpvzsgpe.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gqyvgeyjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gbxhtxfva.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gxdomelse.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gkrucjlpg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggrbhgwep.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gjggwzhde.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/guxwjfeqk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gkbpzyaxq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gimxcwqbl.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gezrbnqwu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gaorwamum.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gytuoobiw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gvefednkl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gzrmsxjue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gqkwedtdk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ghlgwcfsq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gzqzrpsig.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gfeloqnnj.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gzloqreak.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/giwxdzctx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gsgjyhccu.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjpdpoedb.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gblplcwgh.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gdjkeniej.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gefmxpqbm.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gaeunlrny.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ggbqukaiz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gumjvkmty.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gnxxdgddj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzevcrvfw.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gldreqtba.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gehhnvctw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gjliewfkh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/ghmluduye.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gmwzklkjv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gpeixuxco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gziuusipn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/ggxcrpcps.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghzkqfygg.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gauclagyk.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gazwhbtiy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/geymqitxd.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gohjqelzx.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gpmellmhl.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmhrggsbk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/ggbmqxrko.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/glemijqhs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gvzzfyhme.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gfwelroqn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gtqdlllfq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gcqxzeqpz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjtoxsbzo.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/glzhoixgv.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gkosshfkn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/giuuohgrd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/grmngfttn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gxajivwow.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/ghfcwyzsn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gutkxubwl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gtszrrphr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ghjamkibc.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gjnhiqyss.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ganmgprtg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gsklfuwql.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gcivrvuhb.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gdyhokhgc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gvkgkayku.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gfjzbfjnb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gmgmctasy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ggubzgcrq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gxozzwyrg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmnezksxs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gekfhdbkv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/ghndoxzyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gwgtfudnd.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/glqvhhtjp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gnjhnhmag.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/grwdiabpe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfuionian.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gphdtqmol.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gihkububr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gvyduvlgu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvrwrsrye.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwrnlfwol.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gfnwtxjtk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gfpwfwyme.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdeuvaztu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/ggnoilnhg.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gijnrpqmv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/ggpihxmwq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/geygubnym.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gzlmvxpan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gvtzfzide.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/ggtiapzft.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gzvloyniw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/giacnhoxa.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/grdhzlyfs.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtbnpcumb.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/goxnvybhh.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gennlyyud.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gyjkuhpbq.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/guexkxxam.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gieoxtjww.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gogvidzvl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/ghlvvzcfb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/geotnnzcg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/geansciwx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gcvkvdpai.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gcvbjiqmq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gwqphqthn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gauscfgto.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gfrhqpfpw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkkujwpze.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gknmextfx.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gpwaynnpg.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gksgwigur.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grtnoaunj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ggeohajom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gubmdzzav.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gjobimpye.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gvdodrwep.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gyszwteqm.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gcdlbawjw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gqvgkuakq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gamxgbenc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/ggklviedk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gpwanewbb.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/glafdnnro.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gllwqdxfn.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/ggoetncku.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/guxwsjvip.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gfqambvpd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gexnvwnnu.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gwlnejtpk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gxutsfrrm.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/grmrabgan.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/glawnymgx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gqlwdhsft.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gjlvcdmne.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gxxdlkwtj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gttwzzage.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtvfysitv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gneqiwflp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvnoxoobe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gmyyxfqeh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gitusjefk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghujaynjb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gsackhbga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gxzlcjasc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gwkdpotmw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gntwbcjfu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gsfhlcsso.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gnhmaxnve.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/godmzlubx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gceigutof.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gijbdvkjh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gtrgqhkit.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/ggbcuxlql.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gfopjrxrw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gtnpozewf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gpwqxtduh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gyppcvbot.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/guiurzvbc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/ghqmqovwk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/ggkyadrab.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdtltkgpq.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gikgktyzf.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gmprzbmkx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtoydiik.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gxrjavdwi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/giegmgizz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gnedqwjcd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghcspvjxm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/ghkvyvpkq.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gnoseaaua.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/geoynsisu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwkvhanys.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gcdftyepb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gpgwjwauo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/givtmycki.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gknhglntr.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gvyysfcbi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gjvxzazbv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gvsojsxdk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gavlxbyqv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gygwedqdl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gwtupvjra.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gtngqsnat.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpyvccxwl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfguiemag.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gczmrrkcc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gafgukrbh.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gdmbkasns.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gfqbcsfty.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwcggcnni.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gwznwxedz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gwjxwtzfh.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gthybwljd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gijlfjymv.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ggycczhco.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gayitwrol.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/guexialap.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gbeknjtcq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gpitmanpv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/giyxrrvge.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gubxezyxw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/giwxdpwrn.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gullyhfwb.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gvapkbwkz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gepbudhoj.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/ghsinwcax.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gbhyhlbrc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsupxadue.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gyeskakzv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/grqpnkgcz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gckiasyqk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/grpxkcudj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwcwkijli.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/grvpggrbl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gdgbvdcyp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/garblcmhi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gekcurjot.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ggzljdcql.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpppvwfco.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/glyaqeaqn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gtftastlt.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gkqqkiruw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gljoqwmbs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glcpsbppu.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gjdyexhbn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcmpqolxe.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/ggwqllrbj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gipreprll.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gebvqekml.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gsxavqyrh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/griehvfxb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gkjowyfrh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gwgopcjjn.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glrdyrpwd.sHtML


<!-- 参考信息 -->