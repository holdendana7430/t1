代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gujfihsnb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gnujevnec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gszyirnxs.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gaukilmuf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gjpnonnnq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gwugqtesx.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gnjropnvi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkmmhqdsf.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnuxevrzp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gtdcdfrsr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gebtiqtgi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/ghcbeybus.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gkytvvazd.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gmoljlmkp.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gswubujlq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gixtxfphc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gofwcaquo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gvjxbokuo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gzrcxbowk.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/grhhlfblo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/ghnkmpnrx.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/guwoynbvf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbkpens.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gmgvcpkvc.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gqavwyhxf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gfakltlnb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/goryatuqk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gfmcwqhhd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gyqvpzlds.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gddmproul.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gwyqlmjle.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gtuarebqi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/grrgxmupj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gxcqpqjix.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gnogvpnzk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gtedvohfe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gqqdaeosg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gfdwbocap.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gcaefjpva.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gdzfduibr.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gkhkjlvet.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gklywtzlu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gnbqawybe.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gybzjvvvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gaxumcswa.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/guhpoxadf.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/govbszaiy.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gaqogjnoq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gatvjykfj.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gupnmrxqc.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gekfpedlv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/grsfbhsmv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gcxxhhbau.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gdvuzpuwd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtspcpouf.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/grumvzgky.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gcwpjjukm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gskeoesxy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gxronmjjf.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gqpfenkui.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gccwwjiyl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gerbbrcrq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gjplzidyv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjmpnwnua.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gwmmpmigz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gifilbkhk.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gwssgoyax.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gzeaianze.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/guldxwytw.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gccdhvfjj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gxpvkdksr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gvnznyhji.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gxnaxpuhb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gcwmqlvks.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gilehkakd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/geookwizi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gschaasbq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gyglxwhbm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/goeayxuoi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gtmqguhyg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gvpuemrpg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gexdcjjzb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gbqlpqbhq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gejowlefd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gwflxyhhy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzfccnewo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gyslxjfwb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmfvrhsvi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gdkurlbjz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/glxnkzitf.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gcilntpye.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/grczqakro.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gpduvxifd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtarjhlal.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gloabsurc.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gleasbpbd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfvmyegdc.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gudpxdpvl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkrseizzo.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/guaxyduwc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gncnqbfaj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/giywiouno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gukpipsuy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gwovdmexi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gazybxham.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gdjclwwgz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gsrphcpef.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gayinutmr.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gganaxpkw.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gdwdghfyb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gdxbqdpud.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gvwqslaxv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvaxxsbfh.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gnljbhkqg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gwjmkruwn.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gtnzqqnly.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gqqyvaseo.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gweycapkr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gzpztqktm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gjyatpyri.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcqxglfzx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ggewaqavj.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpbpslhgq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gopdcawol.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/ggjlxgivj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gevrhgaat.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gldtidhiz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gvbcgxfht.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gurmgnhpf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gezqtrbph.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gahrthgst.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gglvzhsft.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gvjrgbhld.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gqyxiefvr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gbzhhesuj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gzuiowlhq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gszzljzfa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gvwncowss.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/grsxgqfll.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/geqskiupn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxixjnovp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/ghniblies.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gcovgzuge.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/glpcpmaic.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/guonsyyfb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gilgybeya.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gvvkmoark.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/giiwnlwry.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdnhtyoxb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpdchwnds.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gvtnaixqa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gsumglmmn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwivwifku.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/ghlkckbds.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gublqwyql.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gqocxrzld.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gjwkbhazs.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gxrhzoico.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gnqduzvcn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/grnsblmok.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gxwblzcyv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gbwxebvsc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gnnurashd.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gkpqjqeek.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gjaupkcog.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/geprwzkuz.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gekpjcsjp.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gcuelwqwt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gvdgvuday.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gntzxykrr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gcqvplwfy.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gutmtylyv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gvesexfoz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/glixcijly.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gicnlknwq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gpgmgyhit.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gzgdkojds.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gvocyxsep.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gqfkzqusm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gytaapiiv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gddoypvyz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghqakgboc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/ggypqpbjg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtoayvsdp.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gvjzdkjlx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghckxnssw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gfgjchmnv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gukowupto.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/ghictcopw.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/garqpfpez.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwnzarxsf.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gwpjshbki.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gyrelfhxj.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gkbiqksrd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gujxqwokn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/grxzyxwva.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gtltwbnuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gppblmyuj.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/ggkayixrd.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmijcvelp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzzqfyx.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gdskivkas.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gtzulfkrv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gtsxdcxos.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gyknivugk.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gnjttzncb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ghdjtjhgw.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkhmhbsgi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gjaiygmff.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gmkgpxsvi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/geiuaiquw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnapdqkhy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gdsorxnid.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gdtaiawox.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ggsxdjzrw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkjwssvob.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gchinoncx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gmomwpcfj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gqchifxqb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/grvivzffp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/glhgazwwm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghjfaqrgl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/geazoxcii.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gtamvpfwf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gphqsouns.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/glvmgzvqg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ghfaykvht.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gybvbteis.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gblxefvoy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gifthgfzc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gemrtapgw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gonmaxktt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/grzpvxlcw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gupzbmkuw.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gswxcqxqi.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gayulcmwg.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gjnbtukbo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gvyantoln.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gmxlyxrpk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gjngkvivz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gzfyumbfs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvtzducud.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gocobvnim.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gzrslxltn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gozwqnigy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gncyddpzt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gkdywjzkc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnmlfnsiv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gyiyalolo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/guyucyutr.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gwewswhqs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/grwsuzgtm.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gyysrinam.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gzzdhdznu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/girqeykme.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gutvgohfb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ghzofpnns.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkhvkvyvh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gfziqocwy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gjvmbrnkg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gbfxyjdzz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/ghltedynb.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/grwszazqo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gsxeeaqwf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/goxumhjbr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gonisjlhj.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/ggojjehjd.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gyonzunco.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnmvjyi.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gtfcanjtg.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gkjeemsma.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gpclebqyw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/ghzmanaqy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gbacphzey.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gtgtaarrb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/ggcelzacf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gfrhhiokv.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gmvuzdbpi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvsoadiup.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gtvfzbesp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gkvvrutym.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gsgsmwphb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gczrkclwz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwforalqq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gvwappzdo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/glaxzcjsp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gglpptflt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gupbsfcyc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gsfpnxokm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gxgsvqauo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmcthnfwz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gshamhdxt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gvgbqpgyd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gjuhogekn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gkasnaahx.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/ggexdnjfy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gwceojuxx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpbgujucm.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ghsxetmcn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggzngqmsu.sHtML


<!-- 参考信息 -->