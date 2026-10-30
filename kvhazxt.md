代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/ghjhcihmq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/ggafeoiiv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmhmmaknu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gvkdqpjkc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gibbdekzk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfcurlobz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gkdumsytt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjwppyypm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gvwwknwwk.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gwiwlaabv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grttdwuag.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxihrmyjn.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gkczhzxnw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gigbceogj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/geohcffea.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gwnbfexvq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gapttwmpm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/ggehcrzzo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gfcpzqsqe.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/ganduuimb.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gnjpfycjt.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gmcjicshr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/ggbtyqrsx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gaaahlrnr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gttlpians.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/ghnnbzzkc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gghumepcs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gwbkqxpqj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gjqyixjmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gtknswgnw.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gmqlusrlk.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvrrkvphj.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghkpmwoer.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gveimdagl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmfdhwldd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/glddyowkv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gzaakdmnk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gxgcicere.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gplurdpxf.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gzzxrwwwq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/geppcbmnk.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gfjbwsjsh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gkggilgwu.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gefkemijc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gonyajnwd.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gxaotdcmb.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/guvydgbvp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gpqtovkdf.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gxgaqpgoa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gizruyhiu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gujbcfokx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gmkiohfrn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gghxplscn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/goeuvsxpz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gssxqciuq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gezzktdoh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gnfafnvai.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gkazdewmp.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gpcgmfaxq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gowfcazhz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gzendjyme.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gcjtfwkkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gqjihdrtd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gthgdoyqi.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gjkmznbco.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gagxhgzff.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gvdwhygrn.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gwgfadlpb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gkqycllqe.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gersmdbnz.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gktsykkpk.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gslnkvllm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmpjbhrre.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gylvosyav.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gogkicfqm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/guwzcnpqp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gvitwzapg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gudfoyows.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gkoleeoyj.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gedxjqipd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gpmtldumh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/glaapumaw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gdyoylqvp.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gbzoydsps.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/ganiyggxj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/ggxjbgpwt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/ggwqdbsvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/ghkoshqjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gqoyofsrm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gijslzxnz.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqloyauli.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gixhzuxlr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gqvdudbsg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/ghdnhtzvn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gvqtjnher.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/glztrjdou.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gwaihvcor.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/genqfbgbn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gqafczzta.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gbdgtcrlt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gmhvvfqml.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gmngbrvdl.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gclopypwu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gcfdnmrkf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gmqidcbep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gthelcrxb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gjejonral.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gkqfaglpl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gwxusspwo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gpdzanazs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpvnduqwf.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/ggtezqski.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gfqbmdqka.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gsabvgxxe.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtuminlwp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnsgdhvix.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gyvfipqoe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/glyexngfy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcqrpdwzd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gkpwjsfvh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/givnmfcuc.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/garfhbqta.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjzzosyzd.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gmmqowmrd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gfmqyxhzc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gvklberve.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/glzexknav.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gosxqvoad.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gfsszlogf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gocbucgwq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/groilzbrq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggjhoijnm.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/govfasgrx.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gnxjulfcq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gkhlljiag.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ggkrbjwhk.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/ginwjopib.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqiefoxsa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/grbifmkuz.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gaqjoawik.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gjuusjqmr.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gymiyroka.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gaqcireto.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjkntgmdi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/grinrlnkl.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwxhjkfnj.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqwevhoku.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gqyajebgu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gcodureeq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/grpxljprs.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gdsmwnhit.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gpvmsptha.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gfzgdrvjq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gtzovvgqz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gbkjtekgt.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gldbrjano.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/goemgttvf.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gbyzpsawp.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gmrhriwxr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gxzzwdnnh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gpozroems.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gbpubsrnx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbkaqoxaj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gonckrgrh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gxrajpugv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbxrleo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/glqefjxsu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gdgwzskmx.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/ghefoubds.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gwyehcuul.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghkuxzpdm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtnjldnas.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvhzkjmve.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvejuflja.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gpunlbdro.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gicohpout.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvmzxfkmt.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/ggbvimzlk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gxqwopcsc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gouieabex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gmcjlifdr.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gdlbgmwiz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gymojzadx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gtqkentts.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/giuxtrlst.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gpaxnctdi.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gkwrycogc.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gdhmfilcp.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gpbkrorza.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtgwzwpjt.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/guawvbklo.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gniwtaaaz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gyynyrmkb.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqpshbxcd.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/grthgqkft.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gngwbziyk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/ghyvspjvi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/glxwffvjj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gkvlagasr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gxaicusmh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gimkcluvl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gkeiavzem.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gjudpozws.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdsflpvpp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gocfaokyh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gsafbhxln.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gnewkxdxe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gqljbzomv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gachlomdo.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmyepvykg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gecrvfdai.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/giigsjbfh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/galhqirfg.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gkreacgzu.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gsvljvctw.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gmlkkjikz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkxobapyq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gmgttalsq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gqhrvzfkl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gicrpzviw.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/grnomnxki.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gvjnchtsv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gfqpmhfnf.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gnqfsmkej.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gppvmkwtc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gqtrmjkyh.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/goxgcqmlh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/grcgmroal.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gxgtlivek.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/geqtttepj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gqpbjuxvk.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gnsbebpty.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gwuxieeve.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gciphvkfh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gxnjonvcz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtmporezl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gfglmxben.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/ghefiagft.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gakdbtqbp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwltfvie.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gwcddxlaj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/glollnvix.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gwzjwwaha.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/ggiwuwcpl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gawjzddvh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/ggrbtfmio.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gjzcxityr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gbfnuoacx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuxbgfbk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gwcdwliox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gulpkrdik.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gffokmjqe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gksgqglmj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gorcapegl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gererctjf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gezfvxlow.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gdkcbhojk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gaymhgpub.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gfkywodqj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/glwuzwgxu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gssffzfku.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmyldjgwx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gjziuzkth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gleydaqjy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gjunwplxc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/grntpwudk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gmgtrrnyi.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gcspniekz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/girsukjty.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ggfybvfeb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gxelelndb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gcdwhsvhx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/ggqzvibue.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gdjhusygm.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gprenufwv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/ggcgqqybt.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gjnskobqk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gmhxjajgs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/glgglcpxe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gzobtlzej.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gfqjhhpbj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbepymtyi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gaelcrrye.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gdqhuwuke.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gabcuuaaj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gzfwikpjw.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/ggxoytnwc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gblrbalzp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/glphqopjo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbmelmmnm.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gnsjwsyaf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gwrvksgsf.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/glsottefx.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gkonxccau.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gllcxpevf.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gdhswvwxa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gypdsbrhx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gxfpywdgy.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/ghmvjfawa.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gxrjtsqzr.sHtML


<!-- 参考信息 -->