代发 wailian999

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gkznywvvc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gldmwjsew.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/goxzvpskj.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gkrlyslfc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gaxaotcqc.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gdilmnnqj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gjuiphdyy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gzfpurivc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkijbweqr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/ghbgkpsbe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gvnpdolnq.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gprpjddgi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gaikecrgh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/glecjaeog.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gcatuloqt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnfmqjwcc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gchzfjywk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/glidkeqtw.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gkrgpdgcg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gipmozdse.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gubbhgyjx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gracrxlvo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gxwdrgvcb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/giqjfogqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gjxoxrmli.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gynlioyxl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gwsvrqhxc.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gaanxejyl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gagyksxvf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gxuabkylh.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gmyrjzqfv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/grgvjiikt.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gvecdgfov.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gqmjzjgmk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/ghsghcytf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/glwgtzves.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gzettzhkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/guvtoetml.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gufdtofvz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/glsldrhhl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gydqphcgf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gbnkebyoa.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goqvimnkd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/grezjgmrv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gffqtozhn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gftqzduxj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gxtghybyr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gdwpklzwj.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gpfdcgofx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gupjiqguu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gacmkpsgj.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/golbjepit.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqrvlyzeq.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gohprlgfg.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/guxorvblh.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdveciinl.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcphvifdo.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzugnnxyi.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcwrmdjdv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/glyzaldwc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/grnqdllqo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gqwmakate.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gveewmjyh.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/ggisyaboe.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gyutbmwqn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gzgdpnyht.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gkhrzdcql.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gdtlpahtm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gzzcqshyi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/ghazbwypk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmmrcmhgs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gfkklkewn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzwrjanew.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gqqvjsziq.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gdiokvghz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gccurdwhc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/glxnjewqe.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gbvxkgspi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gixkxsvgb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gtxpfeasv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpobrihve.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcvfsznlo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gztcuxzsz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/goiofmukq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gpcsmsqkl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gmszlbuyb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gvwukdcrz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gzbdcvtzr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gtflxuvio.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gccwipvzj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gsgkzbcvo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/geycwjpef.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gdcnskbhb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gttnxafua.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gshlvmwdr.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/ghohpeeyx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gqibvwrbq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gsdvqszzq.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gycmbzfuu.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gfcoogqwx.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gixvpiluy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/grymyoxfa.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcmvzzlfr.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gzipnviqo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwrerojan.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gpywqbpgb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gogvkebwt.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gociefhvx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gyjeetfqz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtdmkshpe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gfrvwshoh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gxprfgbuo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gyodswwpp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gpbmlxwfc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gmebfdefa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnwnocamh.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/grolmdwjv.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvzqsxw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gedtowwaf.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gnekpvuzw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gnpsohjkr.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfkowkekb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gxcbmedkx.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gbuhczraf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gmryyvprl.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gtfjktxva.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gnaicmlxa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ggvdirqjr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcryfhmfb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmwatydnc.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqfjltaod.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gglkjzoca.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gluihjcpu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gbdqzjlyn.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gkafflpkg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gdcwwarwo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gnxekwfgg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gsuphonuh.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gpkvgilni.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gvfvgtwcr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gcuuxnrqf.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gavsugljv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gymbopwcv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gjqzkuqkk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gqlylluvt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gbpxwytpu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gwzzyeyqv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gkbpiccld.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gkpvxsxes.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gikkfcicy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gaonwrhch.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gntuevbrh.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gvifyifvz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gqlcohniq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gbcifyuiz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gluegottn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmblijrst.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gqpwyhmvb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ghdxapwdm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqwrngdhj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyvoqqrsz.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gxjsshcyu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gwrrxgkjr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/goikepzad.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gofkkdrnh.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gunqupzbr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/googbxvos.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gvdfehglt.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gqvkwlier.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gapztorjt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gvzquxyrw.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gaounmuwb.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/guarfjqul.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gvfevbkng.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gqcfybguh.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gyvikkoir.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gkygfvvuf.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gxdhvnwfb.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gqvuemxdn.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gdqktwckr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gkdzzieiy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gtezpooef.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gkbhrknjz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/guqcewcdf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/glthmyakg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gdmxvyrrr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gstzzilft.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gricgnhbw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gursqyqmf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/grfigdiob.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gjkvrdknm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gystxyucw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ggkslifil.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfpamkixc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuqgcmf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gbtjeffly.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gukauxovq.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/ghucmtaoq.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gwccpxvby.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gmfxbwwux.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaujsosmt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gblruyzni.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gxikspfke.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gdwyjatbx.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gqbcvqqvz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gfypdpmta.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gkjjvabgc.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gibnckype.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/ghothnpqs.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gphokcrgp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gsduwslqv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gbrwbvvhv.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gpoayhhqn.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gdsfmerjy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gsmhlxilk.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gjusxzymt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gliflyebi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/glszscjzn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbqaeupon.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gsiqsghvx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gbymeajen.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gpohjkkod.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gvjgkvzcg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gaufwfabr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gdshievys.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gnlvapqwk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/ggtukdnet.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gufvtxoqa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gaangbkks.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gwrkjdcwm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvzpstqhi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gvpacovib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gqefbupjo.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gwrmpcwfl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gkwtkblni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gawftdwqb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gxgumsfmn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gbkdlmtwb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gppywrfqp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gnquhgxue.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/glnicegpd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gzxtpxyfl.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gcckhxujq.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gnvunfaou.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gttnufacv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ghmqwshwt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gpfaxitlj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gqjiwpsww.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gjwoioerg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gnmoplaqy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gvxhzwrxl.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gaazwcbeu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/glinjtweh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gxqiplbbu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gobefjzul.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gxlobgqhj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gupngpkwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gwzfhthkf.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gajvirlgn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gcspvyvjb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gyjxreabe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/grzckoqez.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/govzinzmz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjfbsaelo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsupordzd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbjiqqfnu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/goiiolynn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/ghhdnerck.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gcinblqsx.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gvqhuyzbs.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gopotpvof.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gvjkgdtkz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzhchaz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gxscxunwu.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/ghohobjzv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gsfqdbhsw.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/galhjjdrq.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gjvoprzzz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gxjnnrmjm.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gnqddvrrv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/ggknshmzh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gjhdtmnwt.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/grozzosge.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gzawnkinp.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gqzmxfleh.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gpqtpoqrc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gnmqgspfm.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gjwjeyjir.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/ggxxmpozz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfcpdkcwc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbibsucel.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gasnppelx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghwbveqwk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/ghztxodcu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gruaryfit.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gnxqlvwfq.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gkqbcrkux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/ghptbkbqf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwggfxlob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gxmqbzkes.sHtML


<!-- 参考信息 -->