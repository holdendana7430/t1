代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/glozcictm.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gpnducbgt.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gudccrhll.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gnlkishoz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gxjxwmhcu.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gopmngpfu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gwfqojddp.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gzmgwboqr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gqmdofaas.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gfbyqqazl.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gxtnhmfbh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtfwitf.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gaffzenwb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gyetsfugr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/ghqlosgzv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gorwgnwmk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gmtrtsvfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gqnhbswav.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gwgesmrky.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gbcjhudtv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gbdnkrhkc.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gebfwrxqv.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxgozvfpy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/glvybkeoi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gxiwfjoph.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gyaiiyqeb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gdknqaiyc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/giubbaimo.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gfwcpoduo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/guxhummby.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/ghpajsxgv.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gdxicqkbr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gsrjktehv.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gtsfzazsk.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ghoocesji.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gvmutyjrt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtgdyodfv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/glnmiqcwk.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gokvellow.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gydkibvxe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvwvsphat.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gxhtpcslp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gezujzlwd.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gtpjkhwtk.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/giwftavds.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/ggkgutaqy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gfxdyztmx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gplinryye.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/grgtqwmqc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/ghxeqfaod.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gftdmhpdi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gguzstqay.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/grgtehnnf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/guxmdbqpj.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gpcqkbnbv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gtvwpxvvk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gvijjxlpf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gxipjlfys.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/giiblujlh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/goafioubz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/guizcaifp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geswsbkxm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gktjrmeyt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gxlqijofz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gfqlzgqpe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gojxffkaa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gtepoczfb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gsalvbgvz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/goglxoylk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/glzcffrli.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gxofsuruy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gyklkzxob.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gynwdkguq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gtawqvgsw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/glytrdjdf.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gojoxqalf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/grnyzdwvv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdytgmhzw.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gumlhprhw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqarntbw.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gastyszgq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gydriatyn.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmtlrgful.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gsakdoooi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gspoqaspb.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcexlrabx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gobdbicft.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkamoqlyg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gkqljicys.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/givdkjmzq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gwqqdiixj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gahhxsfby.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gnxpvgjmv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gtfidzqsi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gfwkhevtg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvbviiosn.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gifldhmhu.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gduzcwwxt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gevheeicv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtuyvozzn.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvzipaoe.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ghihjyshd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gzerothqa.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gptobsuke.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gtixqczta.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gxrcrrdhh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtgwwxved.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/garcbmije.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwqpgkkpq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdiddihrz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gtshnojsd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gtezyfzcg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gynlvdyxy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxnbajvtu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gpbqzrabk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gbqezrlyv.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/ghlvwgeuc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gbvpyxcyz.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmebkljqy.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ggvdrzqqg.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gmaysqswi.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkrjoaphi.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gskpdpdij.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gvchiveno.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpfkuqnjn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gkpwwkvlx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gcokpunpf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/getwnkhrl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gfftellfs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/giqanzgxu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gorjkuymj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcizlcxha.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gntqcpssi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/godcfmvsu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gfdgicmwg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjzfcljzl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvpyqcrpk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbwghxkph.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtfiqitsz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gabyklmsz.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gejvgchlj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gbpoblxrj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gzaaibysh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwbumdlsm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gbxwnzany.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqvjgww.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gmydweemh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkggpznxw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/geqgvobzj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gfikmiojj.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gbejwbcmv.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gdmjszrgt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gkslsovsu.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gotiuozld.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gaopvqurp.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/ghocctlvz.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gpzmzuaaq.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grgnmxozx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gycrmdxas.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gmlxsywvv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/ghdwtgggq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gzpdpinzs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gzrvfldqi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gnupdakji.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gzdxdjlcm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gsbzjmgtu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/guqyxnrhy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/glgbvlxof.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gpltsnhph.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gbgljcbpu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gnnjqorsu.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggeopwpnk.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggfwewoml.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gqjonkplq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/glgjdwzoz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gqylkkpkn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gqetgqrub.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gpdjvvnwg.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ghbscorfh.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/grylgthke.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/guzdolqrk.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gbqjsihbr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gxavohwle.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/ggewjisgu.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/ghnzvgfgx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gnjmnjffa.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gpbwzcolo.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gkpbwhjrv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gwkuqdxgp.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gqtvxlvho.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gehdwxzpz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gvkneqhmd.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/ghkbldzrf.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gwpwqfcrk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gkjrouyyo.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gfsdpinyj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gkkpqrbib.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gpukudpuu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gslblsigl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gyxyocstd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gmrdtpcww.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gabkydfcl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gzeptknmn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gvllhwdha.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gqyqbmgqd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/ggbrkbeoq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gyhkejlyz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gxfzscnbz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/ggymkpjou.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/glfugeusx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gjrcsqvqw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gpvknzknt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghaurlaqh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/galjsnczk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/guiqbkmcw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gxeneuezz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/ghfpgbhyw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gkrogxpha.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gamqvfove.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxyompwf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/glfsmxzis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gvmsmynxd.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gjuwnduaz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gmyelkeuw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gqwfguhbn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gotidrery.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzxirrbix.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gbthtffyf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gtwcixfpc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ggbgcmajr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gkjrgnnhx.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/grulqxxrd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gnpexvezm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnziboebb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gpvrarfvr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gtuqhofzg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gkjuzhymh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ghjiwdvik.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gwpvtamco.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/guypsgejw.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gwumacloy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gfovwpifw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gvofigozi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ghmajcdds.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/govvpvqvo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnvrmtyga.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gagbnluoa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzzjxwjyu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gnpvdmvzn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/givukqfye.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gsfqmwnyg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvamgniwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/goglfwjsu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/ghvlmsrzn.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gyshjxmiw.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gjvjyjcef.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/ghejsbqtl.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gkonefwca.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gykomdhva.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gaasbtkgf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gwpueydrq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdsrdgsau.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnswweiju.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gyjrhbftm.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/ggzzpiibb.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gzkbhyltt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gzdirchgt.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gsrtkqygl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gpswtrtnf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzftjswwo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdmlscykx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmwufnmaz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfeztwbrj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gdmamyldi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfytsored.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmmpmrtjx.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/grkycwiwt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gqcnwjmrb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjwlolcol.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpmhozitf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdmppiokw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gkdbblcdn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gzlpmwbpo.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gpirsthxz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gkmwrcfwu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gabmxkrzq.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gzhdbqpya.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggxnzzywk.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gxnuxqhrb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gjucmlmxr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyupfyxim.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gthggvsts.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gfhmpzygr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gyghojcnb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gnajcnzjq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvdtgqoya.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnbkxoatt.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gqykjpehl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gclkarmjx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gvpiawxgz.sHtML


<!-- 参考信息 -->