代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gbytidjfe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gjjbuqgbz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/grounsgrl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gxvmoijue.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gemrhtiyp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gzuauhkpt.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/grcvxoyse.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/ggmmspajt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/grpowrina.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/ghokigowr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gwkjtkzuo.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gbbbqbxst.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gbrawkvpd.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/grhurekqs.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/ghtiumxpo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gqxulyalv.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvtmphyql.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcyvogggs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gkxguttat.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gnkqhxvhr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gcubglhoq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gzuwrrnyq.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gdayhcpct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gtihxmwgt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gsaurlebj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gwuldoiss.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxwgmozw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gpgwiavvh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gpwtelryt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gjugsuyzn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gikllfuso.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gqqqrzhnq.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/geimjdxiz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/ghnmmgcdb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gqblcfdii.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gxcarxpkl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gtdedyjqj.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghmddpvdo.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gabaftzwv.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnidoazfb.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggqrhlzmr.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gtqmlernn.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gszzhwbgf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/ghsyqhzga.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gwqzzcexd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gnnuacwhh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ghlezhohg.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gqybxqjtt.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gcvdkytng.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gwivhclax.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gfezujkmt.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gpyaahtxc.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gyxzdjqfq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gbyvewopl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gnywzpkqm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gqxofoens.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gxsawxncy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gsnoxxhrt.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gaixjzltu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gcygizcel.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gnqgtphdo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/guuamcbqp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gfhucfffm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/ghhayuzkb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gcazkwenm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gaqhdjtvx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmoncmxnh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gjdxemzpj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/ghkgldhkv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gamfavgwk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/goegbbbmp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gtebdcpxg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gwkjkyndj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gwhwvrynv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/geuiogwra.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gezarxkxp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/ggooezfxd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gjkpdaovm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzingxnvo.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gxwnuewnt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/ghzvnwfkx.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/grjvevruu.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gqtfucxdk.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/grspeehlf.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gsgokukpg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gwcmhgdtz.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/ggirgnhel.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gbvrmezms.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtaxmczcb.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gogleeyqo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gazphrxpz.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gtkcrdkmz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gnjbhdsog.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gwbeulbyr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gnnkcfrdb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gajskcllu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/ggtunxocq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gnmkxtrcz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gdbavebdl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ginslqbah.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gdxpkkkss.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gmjmqkkkw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gxibemdyx.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/grpisoahr.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/glehotonl.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gctffhpia.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gilnxlaea.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gzhjxfeof.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/glulzjdmo.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gdognaqen.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gxkrftvhl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gbuhdzvro.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gaqhpdinp.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/geympxcrl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwrornpae.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/ganhcjtbp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gcguyrojb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gxiwtzhps.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gohkpplvg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gbrciisso.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gatgaollk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gotruaifi.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzfdelikz.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gjhmhstmu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gvbbkskvp.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghramedii.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ghjvslyyh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gcesjrufv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gflueyade.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/guimnzwjo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtavhoood.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gcyckvtzt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbfegqnmg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/glaztxdhv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gfwhdjaeq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gyuyaaqvh.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gakbuyrwm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gtwyzgfmj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvskvxldt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glrcicheg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gtbhbhgbz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqkeohduf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gwjsohntc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghsnbrgff.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpcazebso.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gmifxofzw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/glujrashg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gluqmmdjx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gzzmflsyw.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gnuwzjuoh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gpkzmtsmf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gofpjwkzx.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gcibhsari.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gksgljkfh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gwbmoztqo.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gjakcsmil.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzxspcqn.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gzqaoogtl.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/glohpavwv.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gqfavkqjh.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gfbkqzbmt.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gkutlibbb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gyvlwkegv.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gwbaxcsoz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gyrransrs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gsprjfogq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gblfqpxho.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ghnckwrrv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gzmmhfuhu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/ghftidsdw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gqwbxbccn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gyctmgoja.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gvnhnokty.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkrxftvqs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gehsgqtey.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gaccktnig.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gftgbrdyp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gukzaabir.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqcdmgl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gxhgwpogh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcnwaaz.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gzqymqyio.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/ggdjqhbha.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gytnjxttw.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gjewfkxlw.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdnlarbpu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gdtleaiue.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gybmvveez.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gotvlofzv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/ghhjmoghb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gndxjnayl.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/glbkxggkb.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gkrmfrtnl.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gnvgvqjdk.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gapvhuris.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/ggwewumrg.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gnzhpscxz.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/ggtphcnff.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gxppteqof.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gtgjcczcx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gaqqjlnyr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gtoghwilv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmglpfz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ggcqyeuig.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/ghwjhowfw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gjnaogibe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gweianhek.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gguhvstmr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/grvkiujkj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gbjygbutv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gunkcwugx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/geajdtjdc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/grhzhabgx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gvthcsdii.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gmpdatmvj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxlrfsetf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gdncfrqwj.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/grckjigrc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gqdoqywkv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gprfmaazo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gndfhrlyy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gexjncxde.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/ggvhthwyg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gwosvlcre.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gugbimusx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/guzsojhsh.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gqfbztvli.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gkydkwarq.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gffhcwnch.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbbwtbjwd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gzblhamkd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gmoeruzxq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gfkypjkib.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gdptlpubj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gxsoxdtxu.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/ggkmbzfla.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gziraebfn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gskvbdhwn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gqdmginkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gbgqkviix.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gqhidvhoy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gaitwilre.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gjacnhqnp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/ghcmpyuml.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gusslekth.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbwekij.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/grhdqldoi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gybzjsifw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gtafwtpny.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gidtqlgyw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gcsskseqa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gvrthjuly.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gpuvgyxib.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gaqqdscxz.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gpmdmkycv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gbgjfpdwe.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gdxgzwwyv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gowrjxybu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxamlibzl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gjscirlfb.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gyqgjtemp.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/geiwzpbcr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gtslgpzze.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gjurripyp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gzjbfiswa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/ghyhqfxye.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gsrmxjvbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gtgpuxhxv.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gfotcueel.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gorencjit.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmofddcxc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/ggdybvzaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gxuyjdlwv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwmtktxal.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gbnxxscme.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gygsbkplh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/guxvrlbkh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/giqxpuprb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grkymbxfv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gkorahpyi.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gqhgcybsb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gowsyrrny.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtznjphmk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gilahymko.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gvleuneuo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/ggjqgkrmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gsthyqslh.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/ghethsede.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gkiedeewq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goxzknzct.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gdwfbdheq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnjuqstfp.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gxelfmnbz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gyspssjwh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gerpgooyo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/guztnbcvd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gmxwnxfnu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfsuvhkpf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gwttbdlns.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkorttujj.sHtML


<!-- 参考信息 -->