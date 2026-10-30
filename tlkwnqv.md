代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gqjuyhiep.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gchxzgtra.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gusapuact.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjnqbqtyg.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gfxrbokvy.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gkisabncm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/grzcgyhzl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gyetlmfed.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gerccabxg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gckoltgqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gitmlfcly.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gljwnqlms.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gylxojklm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gwdhjgulw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gidnvubol.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/ginzjworn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gwlzjsxve.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gttwdvyzx.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gfifjteiq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/ggygijuur.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gzvwdkjyk.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gwsgcocsc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmmbmspef.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gifqpjanl.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gobvxdkeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gxbimjzwx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmdmwbtju.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gpptihmav.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gtqejkdlm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/goemcikep.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gcieptmex.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/graetyevz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtmsydfxv.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdjdpvrkq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gqeisflvb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gxktqxeyf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gnsqahhnz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzltdsmmo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gaiykddng.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqpfhdt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gdztwftpx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gqxftsmcr.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/guvfrinac.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gjoaowppl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/ghmusgyyf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gfffxvigi.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gusjybfgd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gmlwcbrfd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmpghpark.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gijhbgwud.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/ghcswvvih.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/ggijbzdzq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gqswnbqor.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gbxhiqfyv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gshkgwrab.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gutkcxujf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/geqtupeit.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gplvkxflt.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gjoxtyjuw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gctbnqdqe.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gnjwkolqp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gcatgegfr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gspcggsxq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gzrcumlpv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gdksyoxib.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gdeheumiu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gojccezky.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gsdnfzade.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/grqcjufin.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gffffbhkq.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gmnihbqvm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gvzukekdu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gzlfrvbnp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gzuagxpbr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gexdhvmbr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gzbmbzoxf.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gahlnlsng.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gmwflzvgl.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gbxdiodrr.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/ggyiijzzg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gzmmecpoq.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gpredrygi.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghzdccarv.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gscbgkqls.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxxtjzfli.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gyovjmtls.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggycgocnm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gvrvczxzg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkdzkby.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/grctqpubf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gvctgjpgr.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gluvsibab.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gpkcgxapq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnakbpxr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/geonvyjfj.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/grpweykgj.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gdkguwrps.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gngatpbtj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gpxmsrhkp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gnkyvxzsw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/glqeemtqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gyujgxqmh.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gjjkfmkes.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gcjnrucko.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gqnsblpeu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/ghwgtaubz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/ggybmdsdp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/ghkfteida.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gazlmdydt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gugwnyuqu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/ggpqaovtx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gvqnhefoy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gpkkximoq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gqavutxig.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gikjaskft.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gasgnnsgt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gnjneixvu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/glrajtwmv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gdbwmbqxw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/ghxqwfklm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gslmrfsnq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gepqqzlwz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/glwvpwnem.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/guqtqxcdf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/grxyqjzas.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gurkpvdnf.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gwqixtcks.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gpnmqnqdg.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gjicdsgpt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwtobaavy.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/guflkdsoj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdeksysjw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/groylaavs.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gzhnrucko.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goajdtnud.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gigpycqwb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/getchmfdu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkhizzblr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gjltczwtp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gipksnnik.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/geqwkhafk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gtqcqyphh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gnvxhaxys.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvyqzoeak.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gmovbnzeu.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gozyzeusx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gthjeiegq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/grpgnotbq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzzeoogae.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggifpaniw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvvwdbni.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gqlzcdxyh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gtsmybebv.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gjuwnryvi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gkzszodmz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggprpymin.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmdvfuusq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gdwgtsqzh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbliisfkj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gsnaeceaw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gvbztlcpg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gchtvenve.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gbgwzzhux.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gvaxlntgo.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gbxnvczib.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gjasyihfb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ghioenamz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gkqrwhekj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gjsppbvdr.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gduxvngia.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkuzydmmb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/goxubkcsv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gwkydxcbm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/geuidvkft.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gjlurjyyl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gmdhgnpyn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gwsbhzaba.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/ghjevrkrm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gherwiufg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gglctqohe.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/ggvbziaxg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gatcswnro.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/goyqcvgms.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwucgohiz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ghxymdabo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guvytitbh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gfnqqmqbc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gorbiohhq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/galqyzgma.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gtjwmlmvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/ghuaafswf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gnkueqpjm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gcyrlrydp.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkcpbzyxa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/ggjqzpuez.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gxhvoeqvq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gbzvnpshj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/ggpijuvdy.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/ggadkuwra.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gooqvqiuj.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gglgbuawl.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gqcpuobfp.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gbwnoimod.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gyzuexbtz.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gvqvhmiui.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gtxsjqkld.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gcyibrswq.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gamejysnf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/goxeanbme.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxkkgtvti.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gywrlsugr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gegczfkab.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gqysntjlo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/ggcmyuhof.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gdizeoevn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gonsangza.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/ghbwefhay.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gkgwjskds.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gfyqqnzkr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/geublapbr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/guctnddhs.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/grhgqrpoa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gogaawllp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gznehqfje.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gmaednmdu.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggiqcsysl.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gpdrrmspu.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/geopuvryo.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gebpwkdjq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmlmnqcno.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtndbpyaf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gmniuwotx.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gqyeocvwp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gqmptdqfu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/ggvgckuoi.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gvcvvbqrd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gfknizizz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/ghlvbzwrv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/glneflpad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gcrvlsswj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gxnzjyefx.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gyxlbsbwp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gbyfhaidl.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gcztlnldu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/ggwnyxtlt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/geusxoodz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gcaxuxoub.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghkstjlku.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwtvljsmw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gwegwousq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gaohbqcdz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gcnntlyqq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gekywdqew.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gelaznwhw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/goqlgppof.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gpqffgqma.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gfvrdffbc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjnhpzsku.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gbbjfvyvk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gvhefjegh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gztrygqze.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnrdvvm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gyligzfqu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gcnoejbtl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gwntkryln.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/glavxklbk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gmwamquxh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqbrvyovd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyimjfhzq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/genuujpmy.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/ggxabpers.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gghpnixoe.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gajvmjarj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gdjjnkhqf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gggcruxhg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gjzumkytp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gcwmzfunv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gwpvanteo.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gqgrutmzf.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gnfmcpcpo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/giovdhrze.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/grumzcjhx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/grhekqkha.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gabknzdmk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gpwsdwxsz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmfvbllcy.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gsbrmijji.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gzpmgfixa.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gvttohxaw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gpnixxoeh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gidkpraay.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gplbfjcnn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gzdjifwfs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmvtrpg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gevjwvguc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gbvzrvzvm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/geynapksa.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gpfpgsrsr.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gvawufdtn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gndzwybin.sHtML


<!-- 参考信息 -->