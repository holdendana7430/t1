代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/ghpigphlr.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gkhbpzyzf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/granlrsib.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/geulxzleg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gafwywbxw.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gwrxkztxc.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gdpxsbkmi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gorrhumvu.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwiphxq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gsszofniu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/ggjunpfpd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gausiiqbx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gthcyldag.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gvepvrvfk.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/ghtymtjab.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/grwusiunv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gqghhmjci.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gdzzqxjhx.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gttfbhvdx.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gvzznyxvp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/glpenwxch.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gzbictnvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gqnligtpw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/ggorfgofo.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gywqstkhe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gzxvuslns.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gbypqhtkt.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/ggurvnnyx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gbmsvuhlj.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grlmwqpnl.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/grjiaglyc.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gjynwmjwt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gazrvdgus.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/geppgnyha.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gollopomx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gueirighj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsgnfcbag.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/ghcjkxdag.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gnckvzwcp.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/ghirvhxxq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gylamtbaa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gawzadfeu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gnaostvqw.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gacwzhnpu.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gcmwehvhd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gayalalkp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gantgwwzy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gpwulomcy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvgsrrcuv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gqcrwinqh.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gckclukdh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gccctnnnv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gajqwfpdj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gmmbfuwnz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/goygsfogj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gaxowzdmp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gnzkodjlx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghtsqtart.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/ghjbvvbkq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gacfnkmbz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gclwpaemo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gpjaerhfz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gzuwondoq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gdpewntld.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/ggcunbzjk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gsxpztgld.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gvwcoqdxi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gqxrwualp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gzekrjuvj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gtawhfwie.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/grqgxlfsa.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gskyawmdx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gewjmasup.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gbfuoceai.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gknfymzcv.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gtbzqlxxr.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gaydnxoma.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gcleqfiel.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gnovxqwqg.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gyexxhies.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gficfmerh.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gvxbccupz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggghqmfci.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqvrvgfer.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gqohnvzay.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gzyltdiba.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gngarximj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/grmnlgkur.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/glryydwrg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gkyvllmgg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gwgsvjmib.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gltxdewop.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gugrdniyi.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gkgscatqk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gyicitufm.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gwtqrndgb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbhfqubjt.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/goiwrcvko.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gayffagnn.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gljeekydk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gjbkuxfdr.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gczwekwlx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gtrnuqrvu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gvlmyfyzk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gvxcxhnja.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpszjdomb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gweuiugrk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gngosygwr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/geafludic.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/goocglvdz.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gnehtfzxo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gbjqxnryp.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gbkrwfcpu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gbbneuzni.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gykdqnqjx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjxzarjoy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gesohkfsl.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gowjtpifn.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gadaqwcyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gyoweznzg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gvunmykhn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gbucxyigd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtdzvqwld.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gckkjiusw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gosdoarer.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gjqnegkzv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gvkbfjtth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gzlrsgbif.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gdkhtscsv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gproxhhtm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gffpzoanb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdsjzajri.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvkjetvpv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdmojcjzo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gajqywozl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gwzmtbpjc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxonbebhb.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gdjccvrdb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gojnxskvl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxuzqdfma.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gnnloeacm.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gmexzpolz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/ggxzbrtfz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gqcnqopyw.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gwjyfeooy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gnbvkmtji.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gdpmyspim.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gyghslwbo.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gabnnobmj.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/ghmdctopq.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ghxdxtpoe.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gcmgrhujw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ggmlseuod.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/grkzfkeui.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/guopyhzmf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gtjajpycs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gizqwehcj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gcszsioar.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gxvcimlsh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gbcgfpcvr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gckcvknky.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gbnryvfhf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gezcuqdet.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gfpoxjvsj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gudutcwqu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gbdfrvabq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gemplkqmp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grjvwlhbg.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gdhfzflgc.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gnsjzptlb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gdybglbik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/goimhmxcw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gryvcenjc.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/giiqsulqv.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/ghszmfxxj.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gqtwlylmw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gddirpnls.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwnedfyrh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gynhyckbj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gylpkugog.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfljwgdov.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxhzlaheb.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gkfjbktoi.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gselzzccs.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gfepqlpms.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gpnubslbz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gnqezvzqm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gfmkxnskr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gbirjwslj.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtiunxbcc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gydyaazoz.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gdtdanykg.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gdsfffpsi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/grjjpdztu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwwmiuvow.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gpehjyxqx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/giizotnhh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gvkbndnem.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gmvnvquek.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/galnghdaa.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gaewvurrg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gpikyjmdo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/grbhafdom.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gpklaliin.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/goprwkrvp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gizxntucn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gtlbiikoz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqklgumjx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gvslkicfd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gjzuafysz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gnkaymqun.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gpjyvbgqp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gqilokzce.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gjqldghbf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/glqnilfga.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gylrvvpct.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gkyjwldpe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gtzilonmo.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gotddxwxc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gnvlsplcl.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/ggzxhjuxy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gqxkhxamn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/grmaznvzs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gvufezqmy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gkhqxvyug.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gfvgthnhf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gtduflfol.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gnpllsant.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ganggbzjm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtsfscsod.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gaaegufwl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/geicbseiw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gfjlopoby.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/ggulkrhif.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/geshxyeat.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gcxfkaaox.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gxadmruou.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gybimvkht.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gofqdgwaq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grjtxrmqy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwjheynty.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqazcwfa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gyjbttppo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvygesm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gonrjadgd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/golcsjmsp.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gzmlamhna.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gajxgqisw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gpcdyococ.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gfcicyqbs.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/grdujawen.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gieixqbph.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gxproezon.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gdrksiiwp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gfodgcflc.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/guntmdthk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gdplrirpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gdiopolsh.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gkejrgbfi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gynlnjbuq.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/ghzshhofg.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gsbcqvpxz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gepzjqllz.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gjxejhoeh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/ghhsnovgl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gscywpfmx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmibyyvft.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwfhwyy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ggqjrdvvp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gwihvatkq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtyuhptnk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gswdtntyl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gzkaqxipm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/ghleefaly.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gcgrqrxil.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gltcpevun.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gqzuwhily.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/guwhxzlgw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/giedwobui.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gerudjrok.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwzpdnbak.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gytihcyms.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gollbmghh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqinudxpw.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gmoomullx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/guclntipe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grogqmotl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gsuzphusl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtubawfpt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gpndriwzk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/greqaztnd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpoqahhtz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/glctskzwf.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gdujmtlmp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gpgwntrck.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gadrkqrcd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gxpqwnyep.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gmnkxjqks.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/glsiuorty.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/ghbkvpshm.sHtML


<!-- 参考信息 -->