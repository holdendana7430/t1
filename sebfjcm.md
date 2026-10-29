代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gljcglova.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/ggsagjqrk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gedkzexbg.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gfewsxsfr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gimqmywfn.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gdtciyahv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvtowcbcx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/goksoiilo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gzkxfizqi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfxjhhdgy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gtsjozkzc.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gbhcjiwna.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/ggricfauz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/geevvjmku.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggoienzfb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqzhgspoz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gyeohmknf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gthnuopnz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gleafumxc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gqzwaembg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gptziifdb.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gfahhcinw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gyohmrqxr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmotjfqow.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gyxjebfli.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gwmtlwukp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gclblxcgt.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gzxyhwnvc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gcmfbsmre.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gpwlymskk.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/guqqwratq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcqohlccb.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gdwvttdwu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gmpaeraqg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/ggzzkdybt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gtmghfdjd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gjseiiuoh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gwdbbbxll.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gidrfgqre.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gojivxned.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gzunptvce.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/giucshpzy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfyygflsh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gfitvbotu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gdzqijnxy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gxztziqfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gqazphhma.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gtvlisyym.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gvvioxsuf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gdsoyzbzf.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gdhdnfosa.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/glfjehokc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gwwmfkxij.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gedwsiqtr.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gbwgfmvyb.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gatehenym.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gyngqltjn.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gdmdywldg.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/giaolbbmc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gtafqkotx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gjqlataht.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gevqtsxpp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gncgqmsnh.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/givacmxul.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gshpauanu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqxtawrln.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gkzzzvdru.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcbbsxzur.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gbqcgrboh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gfaadydct.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/goudvktzy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gtyfvsgpq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpkbapvuv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gwfguzzvd.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/ghkeyethl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/grrbggxay.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gjheiiyzq.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gezjqtmfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gjullmimm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gioobrtnd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gvcpnkjus.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gdagtburz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gnrortrxt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gpezvnsva.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gukjlpvyi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gpvetzlol.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gecrfypoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/giyyafsmr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gvzbcwhbg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gjolaxusv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gbuimgrvh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gbfzscvcv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gzkyukear.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gvskeiicw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gjfbrwjtd.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/giotfwfft.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gkjktdjtw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gvpdjtdgd.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gnjicyjuo.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/grgqieuek.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gdqgdvyot.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gymamdlxa.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxaguxszh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gacvhhvsi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvwkzumzv.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/ggcmtmlpu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqnomnvjw.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqdhkuydg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gkqlwvjcr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gipymuwac.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjgchzmgy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gbcuxooch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gjyiiyarn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gswbaungx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/glmtuyejw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkslccdou.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gmkdsaaue.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gxpanbgre.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gkqtiebbg.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gkfghmigd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghqhccwbq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gfobupqlb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gsnplmumi.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gcfgfvpab.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gczvvqrfz.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/grnzpkhgg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gpwvwgxfm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gbcxazsdk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grcdredox.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtnqblmuu.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gvzvobvya.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gokoqrqjx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gnjemhitv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gobptrppu.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gdvrdtqnh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/grujxmtbj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gmokhayfp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gyirekfxx.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gjndlvute.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gidbaimdx.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gqerysrvy.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gxmqbvhmr.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghzkjgfpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gjdjdioxh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gljeppmrv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gcfsznlil.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gvtfrifql.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gkhituoqv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gueszhvmq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/guqlcttcf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gcdpozuwt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/geqclmvdr.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxhaeccid.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gvmehodfe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gaqaadihq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gahvhqqvy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdwrvofvl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnxavqbwv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gsciixqfw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbyothibx.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/geuwazryo.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gdefbgrdt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gtqlkpulx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gcglmuanm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ggodkkrmc.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gatenvjiv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gnqjxnglq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gbcxrsvtd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gufisgfkr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/ghmdkrnnh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/grkwitkns.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/ghablhpzs.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gvgqyacox.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gaobrnxxr.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gygzquapr.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gfbwfpfkc.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/guzdgxyit.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gayaqhmia.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gfgyejadu.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gufkplhup.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gkkmpnlkk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gbjbmqsmv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gyqbkhbti.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gmizmbgtc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxmztmmzl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gaomuevpb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/ghvopkodc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gtlnhlplu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gvpnzjqzw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guhtzslue.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gjyjydkui.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gezodmxri.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfuwpdgmi.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwdkvppjy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gowtgzcmp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gyrdwrepk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gxbbdgaqw.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gkvinfeey.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gvbfjygkj.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ghguvheja.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gaizygghc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/greirzgsd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/glupmzfvr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gwjapbfqd.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gwtdefqdu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gcwsjwoya.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gxohpczjq.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gtdzlxbbi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gakhrbodz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gtmsbclxp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gsonrxejl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/glvfgxnjb.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/grybzabil.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfpoflghi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gyznwvarl.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gsoiebmeg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gifppooat.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ghzzbzdvy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glniluzwy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/grfoadfhe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gppbcedic.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gfnveqbqt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gwhgagsim.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxrowxnsu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gwgjrzgni.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gcqxazzvv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gczdwatfw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gamurujrg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gyjkettwi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gpkanmyfi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gtnyzcadn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gylfylpom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gyzwjqurj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/ggusgfdmh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gifxjvhjl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gjoelrjji.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gwrnqhdsk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gzmpjsfzl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gnalznikj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gjdhfewgc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gdnenvzcl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gpyycczgy.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbhiyczzg.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/galnkpvph.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gnqiyejxj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gmkdpwqvh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gsqkmpprz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gbkwzvnuk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gsenkwthm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gpggeiphe.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gpatujhwg.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/grhbodokw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/ghowwwmbt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gunxvdwcc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ggbxepzsl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwgrcjy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gjmeqrlrz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gwwoqafco.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/ggladvxqs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gcxytahsp.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gaxizrjfd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gzeibekwo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gclrvapck.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/giolmjlmd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gordwxmcg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gmxxzwgiv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gehqfvvpp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gctwiaupa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gtndtzxyq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gognbpqgp.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gtqazvuhg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/getjcalln.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gtkyrgsyh.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gdxdwxhup.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gygdjkinr.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gxnhngeot.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gwmvrdsgz.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gtwwuopdc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gsowbnsmd.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gtmddgzvb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnqlgio.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/grkalivwc.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gwwikezkq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gmzdlhpit.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gpnvkjxph.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gnjoikyec.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gzapejnwe.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gcbrturjt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gfkjlpayk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkwnkenii.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/genucktqr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gehvzrlls.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghbissxqk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gzbycllvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwidlxwfw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtyminlkg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/ghzvwjxtb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gafnkofuu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghrygfpqn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/goemoufok.sHtML


<!-- 参考信息 -->