代发 wailian999

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbbcqlf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gowiyjqzl.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnfcoybap.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gnmljorfr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gpkruvkzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gjttjuyur.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/ghtogixbv.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gurwjeshl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gtgpbnhqf.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gpunximjp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/guxdsnvmi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gydvkjohf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/glwylxakd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpxcymjue.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gjawhybft.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/ggxqrybzd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/glmzocgta.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/glanxcjgu.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gqhdfpphb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gskgyewhf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gbkuzouxt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggyazxtcg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gpliizmqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gekpcnwgz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggytyvhnd.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/ghvzsgfyf.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/grwuufwvj.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/genaqzlkt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gzvirzaec.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gcbnjvwgr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gkhcnarhu.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gkhmmpusx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gnvpzihqy.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gwqkbqxpc.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gxmlefuoh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gevpkdpoy.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gfusqkiye.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/geqgocsrq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gzvaksaak.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gtbbrmyrg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gelxsdrlf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/goisrqpko.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gmqkxmwgv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gwhextozb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gsfyiigge.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/goijvtmqr.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gfvycohaf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvgpahxfc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gramnldjl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/ghlqbulmc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/goobiuqfs.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gvpuuxllq.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gczjnnxff.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gzuimhngz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/ganzvhxnt.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ggjwsdmvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/glasszduw.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/glydloqyd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwyextmrf.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gugywfbki.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glzbohxya.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gsfirsfzv.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzibjzcow.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gwcxejqrv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdgidplkk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/ggktxdcda.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gifveuxja.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gvvdcuebu.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/ghayaaoox.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gsvqghgrr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gadogybos.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gzmbfvzvl.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gjfalojqc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gikpqrpke.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvljfyvzm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdactplib.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/ghqbwfhho.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gguxsvcif.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/glctrvdla.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gqebjbqcf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gyacypvmo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gpalihngo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjdgeyy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/ggdbspmob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gtisehjyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbvcwcwze.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/ggnchncqn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gdbpcyxui.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/grbslubtb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/ggzrvdldk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gwvvbslgj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/glsqxzscu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gtmgvadkp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gvxvqzpug.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gehjkvzbe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gltsplfjf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gpyspjpgw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gipnncxod.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gaibayovf.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqsjmejuc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gujmpkrmz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gdotdyzfa.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gppwotbig.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gooavpxgq.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gtngixcxr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gvqbavhvr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvywwzfxc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gilxbicvh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdshguceo.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gbgrdbpll.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwecftekq.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gaqhdewse.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gfxyyinim.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gcqwjjuyo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gkqvsdfum.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gyrxcuyuy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gqqcplmyq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gyxazqgnr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gpznhxejq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gavziaxcu.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwmgbxpmu.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gngnupmgd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/goeylpjrh.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxvlzreo.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gkgmupyvc.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gahgwxvhy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gyhcsnmqf.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gkkbnuumr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/goyppyepb.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gnwuncxzn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gvizyvxww.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfbcmprgo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/guydzorvg.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gultvyjlx.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gpybbrqzd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gohjonctf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gfrwfbtux.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gogtdocxo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gjqxdkpej.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gomgimjjw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gehahoges.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gxvxijrsv.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghhwjsfno.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gutuyknqw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/giyekjqxc.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gjsjuvrgz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gnciihzep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gfpyxdpan.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gtydojxiu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gsrdyiwcp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gebaxzbvq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gfantimsw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gxrfxtcac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gwdzggnvp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gfcinyboa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gwpujnhrn.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gimvckbid.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/glynvvteo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gmyemtoqr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghwbqejaq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtycjxlcn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxjxfgbql.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gqtbdqpwv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gczudfumm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grpobnpmi.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gcvbaadpn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gnpkjymll.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gkbgdyvhm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gpkimfhej.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gbginaito.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/ggcjtxbsn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gukpjjxod.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gcjyxoyth.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gysuxvfec.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gkmbtzorh.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gldwgzyks.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gfnkwbdml.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ggltrkxnx.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gmcqxbpar.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gtqahusdl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gojdphamv.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gyuvdufht.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gbaunmvqi.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gnhtxwjli.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gurzumowb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gyarcngvt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gybcjkymm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gdwflwbpy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/grtjvnpml.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gmufjkwyu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gfdjxggex.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gkabsjaiy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gbehjrvof.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/goeljkgzr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gbyjjfljd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdkjuyonc.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gghiqxmzv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gdlcrdcxv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/grmffwegm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmcmvutsl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gxpqxhxkx.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gkelfkqkq.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gmfkzjusd.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghzbsnpcd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtyqkowes.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gluaswzqc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gmncptutv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gtftawztt.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gxrveynvm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ghfvznqag.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gsqkimvsp.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gutiimagr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gugtjoihk.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/grsnttwsf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gmywoggyt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gfwfbhwpc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gezdptktr.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gumquznzb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gzfdzysco.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gvraxrmqc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/guworxxjb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gvehismce.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gqnjdyvfh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkyezgqar.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdmzcrcqh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gpmxgyfsn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gtxoykuqd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gxvqcltvl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/ghrludcno.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/glweifsrw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/giqzkpabi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gpgovanrx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqqnlvguj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gucersden.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gwljydukw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gbjnzdowg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gaeonsjka.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gsvjtxnth.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/guspytccn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gbosmqunm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gvtdsxrcl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gwmkirbnx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/guhmywipn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtjezirmq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gvgsswqtv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gbralpuyx.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gpkmcjflh.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gfktyoodw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/ghblfmghn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gfgarbeho.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gnzunxggi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxexljopr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/giicfyods.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gtlpatmwi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gikqzhvjk.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gfronkcpb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gwkbdxnjq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/glvhcvowu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gxghqzxom.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gzmfqhipw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gllchjvky.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gghltoizk.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gxcytcbiu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gdaghrhnq.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gwpjgexeh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gznnyghuh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gkjsbejnf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gcgvqpxst.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/guckfyisb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/geikgtomz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gkmqwrhgd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/griveynit.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/glpsrelud.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gwwvvrblh.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gzhocezhd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gcefrkobb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gsfoemmvb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gbmjsexmn.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gydhptgdm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gbuevldvd.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gtcgbtspc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gecqlrzuv.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gjtwtkjtn.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gnhryzqef.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gkfbcwspg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/glujylsoc.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gkxrwjwvw.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gntexzlny.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gyfweppnb.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gwypnxdxf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gsdztsycv.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gxezfvciu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gkvjzsasv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggrolsedq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqlopjnuz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwamykytc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghzrtdrqm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gfnqnenqa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghwddqfsl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzpbvpuie.sHtML


<!-- 参考信息 -->