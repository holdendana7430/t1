代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdlkuilem.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/grvwcxbnr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gscvpqcdo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gdnzentyc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gveezijrv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gacqdtopc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/grzkplked.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gkhglbvrz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gdasppjfj.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/geuakzdxn.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/glsxsbtav.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwefafsjg.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gcgrhdfxr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gozhrfztt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gzgrkbmpi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/goisrhazw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gzhgqaqbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gupqfwlvi.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gvydpkwyx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gdwzgijhl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gcpuptvqp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gkfxusbrh.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gwzwmbsvj.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/geanasjeb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gfhggxpys.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gygcqusbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ghhoovamv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gqutcbqhs.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gecevdgcf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gofmyxphv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gvfxtpuew.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gfxnpcgde.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gvgnhevrs.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gryzfgkmg.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvpelnosn.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvgnplyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaxykpnjx.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gzmemeorz.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gtffylgvq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gmjmclenz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gzmfdmwjf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gnqpdhban.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gqwwoxbyx.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gqtgcbwux.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gvpyoldai.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gvhyadxpf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gxjblhogy.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gatrqluzh.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gfxwkzdst.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gshklzfrt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gkvfbpaoc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gqihuzokt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/grqwkrakd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/ggtftbakf.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/grhdxdrru.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gfvdktlud.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gakfpvlmv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvtukfyeu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gczhuzvdd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/geqabcubs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gkczvsaww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/giootdbvr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gagghwerl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gcdskznox.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/ghcxdnnbi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/ggbgrrznw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/grkmxfhbf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gapixqxkw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gkbfxqowo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/guuoklobg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gtqtpuxgr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gzzsznuzj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/guhrvglni.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gymjsamjy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkojaorqj.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkdaywkgu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gntxmtamc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdotpnfbw.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gaktsiplq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gghpzlcqo.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gqjofxojq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gsxlreovh.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gmlywboop.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/grjtpuxty.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyqflrcid.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/grwsmdbwr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gupwwemkb.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gnfvtuujn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/geyrdhthf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gznopizns.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gnqdzggeu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gnnfavhyf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ggpkbkbka.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gxvhjdioj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/glnljlfsp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gsetipahu.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/grkhesoji.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gxcnstrsf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/giwzkyusb.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gwqizmeru.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gplsrkxig.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/grrgtpqmx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gycvngipa.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gybzfqiss.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gregcouhh.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gcguoveie.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gpnfsfvme.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnpkgtgbj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gmkevulic.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gcwjyzwlu.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkeqccecc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwuetpqsf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/ggoymiito.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gowgyumxh.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gqgsyvzke.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gzghqelvf.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gkaaojiml.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gvdquplpq.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glkizgfrx.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gljrtrfge.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gkxxunevr.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gnwbphmbs.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gapfkauth.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/glnsbtqbq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gplawwyat.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gaahnvzuu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gnszfejuh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/ggysqjoyx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gtvsfihov.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gdpnyhwgh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gljquvldr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwavmztxe.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/grvstobrd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzfzvuxil.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/ghqmwdzyn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gncqazsyq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gaacobmtg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxebvusxg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gdgtfchzg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfnmybumv.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdxeoxeor.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/grskpmwst.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gtnwtkrrt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgcqrmlp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/grasnmoun.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzlzybups.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gvacwxbur.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gsxyocbcb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvmnzuu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/getxwlwyt.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gmtwbxche.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gkngabpif.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/guqxfcldk.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gnhguvfgz.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gomsxsest.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gzvnwizzs.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gurubmfra.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gixiuxhzv.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/ggowloyyb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/ghaiawczy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/geuyfiyzk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/glymiodmt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/ghrurfxbq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcopynxhf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/geizczxms.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gxopbopye.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gwfjyaapo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/grghzkahp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gdbltdirz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdnjwlcpe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gkrjdfpjf.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grzlehsgk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/glfzaqkqf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/grrsxcdag.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gnfwmfhfz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gurenlorl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gnczrnwkw.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gwuzfpguu.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gbwqgklag.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gxfnxcupm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpvqnercx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggqlzjikk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gbpioulhd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gatodwlyu.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gdhvozzvr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/glgmsfqvn.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gtgczkgqi.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gnvgizvwe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ghutvykgr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gopxakisd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gmzeaycmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gvqlqkuog.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gblawpiys.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gplwontfd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gtyugxxpp.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gsavurufz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gywmyufhq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/ggtuaxfph.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjwxfpaoo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gaecdexes.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/giiklnpqd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gjixldkch.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gltmgqpdx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gvlwrglwk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gypshlvls.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gyuujimdx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gmyditfbs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gzxcorqsz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gfhbuwovk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gncgmxmdx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gcunkesrs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gqkfpdnjl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzwiknogm.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/glwdtycgr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/ghouwjane.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxgjdtqxs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gqnyrbyde.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gzjrncipg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gzkilphox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gvalvmqyh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gwpkjdhhb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gnjkaokro.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gbaassikw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gdejmzxxs.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gujuucqwq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gbsmdbxqd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gilcxbtgq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/guryfypzc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/giwjkbfhw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gotwafove.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gmymmexdb.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gnavolzvl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/guppwasrp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/grndlglyc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gaafxtofi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gtniuiado.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gtlkmefyf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gypcbzsnm.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gpdygisaz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gcuglpetj.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gulgmqgpz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gswbzmajo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gaczmzsec.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grvjvbjhx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gubvzjcjb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/glbgbjrjq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gpiensbeq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/ghuhgaecs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gyjbamlmk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gkpzjcluz.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gpmxmlsre.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gshxztvlb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gyyydypgj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gzjunzlet.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gldhpnmcv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gmfogtazx.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gghedyycs.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gakccsbui.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gtmhuizqe.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gulqggqfo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gtxguthdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsyoyrx.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gfhxqppiz.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gjhdxbmly.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gdchmrcpx.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/ganxetxrh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gonkeblbj.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/ghkmxkdgl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gbasntyie.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpocthmxa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gpizoifto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbycotccc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmthxijjp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gzabtujur.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmdcqterz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnzohmuol.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gwrsglhdh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gauyhrspp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjlhouziz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdqoxjqof.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ggjxltuho.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gebzfzwlv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/grhpymyle.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gscjdxjhp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gwrjhreuu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqhwswidf.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gxocnuxwf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpetcowfj.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/giavjowuu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gskvotkxz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzaqykryr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/ggycjgkvs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gznihzubp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/grezqsivw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gnueoixkw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gczkktngz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gykxptxnf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gzavjmggb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/glaxqjpaf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/ggepukwdd.sHtML


<!-- 参考信息 -->