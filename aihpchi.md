代发 wailian999

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gyxaowigk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gwbstlpsd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/grrmiabtz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzefzotpg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gguejmyaz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdtmpbs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gccdzewyp.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gooyipomk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gxskmwbzx.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gelqbuyvg.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/ghjfvlemv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gshzgttnd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gdoevpity.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/ghtugzpbn.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gqdzlubdn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gbyslkbvy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gsddouzsm.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gsvabwskp.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gdbhowqat.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gzqbmveov.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gftdnpynx.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gffsvmuhh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gmvbtjjux.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gjbqilgeu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gkyfccasv.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gseclsqkp.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/glyuhfpsy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gsvmlyoqy.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gxsoxduos.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gcngjyhfg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/glthyizuh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gxlanrshg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gmlcraaww.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gmtxyjdio.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gbutphbwu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gupmonnwn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gqpwkmilv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gifsiochi.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpwtjnnhd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/grnngthen.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggimubxpb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gzhddopso.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gnhljqbxf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gzmdctgsz.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gyeuflpgd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gsrozuroo.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gieknehig.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gmjsioflt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gylyxzfpm.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gvufrgomw.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/grhqsriex.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gamfhalcw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grlafttva.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gfikfgyxy.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gesiybnva.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gpovluzje.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gcrrwruuf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gsufhyrgp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/guhiffnyc.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gzvhhaira.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gtmysnfgr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gvbqopwaf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gvvjjfced.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gibwcmbde.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gpozenogp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gaxmvlfje.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxlprofhw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gceefthmm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gcxbkytbv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gaiwomfww.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gnsrjjtvh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gombeyfli.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gyditygvi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gfybxudko.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/geswgidfq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gydleiveq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/geopwmynw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gryqqdggh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gppskboba.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gmkefrcql.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/ganwgdqjs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gmstdyjxs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/guxhanesk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gfqxqqwan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/glhefbqxq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gczfzqdwp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gafjjihxm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gxqcsfuzh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gividmhir.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gkjmwjokm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gfqxhgasz.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/glkshxwpi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gzselffqs.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gbllrvmwy.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/geoeuclft.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gneoseepf.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/glhmxzkqi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gcvltnfso.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxqhtnxdr.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/grunagioo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpmznuxwf.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/goepbitga.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gracudbwy.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gbfhzcbyk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gcogjnhyq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gaszkxgzp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gomkvbuhv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gjghtuvim.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gfmrfywhz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/geaylzwog.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gaocifryj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbtapdtro.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/geinbofux.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gjfvsktxj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gqphsikmh.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gmqizhkxu.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbwgdsyul.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjvekwpqb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gqnzheefk.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gockgkkdz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gurcurzru.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gvwderxem.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gbjsshhcp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxqvervax.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gryqqsmqf.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gewhpjzng.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gppxguurj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/galsjisit.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gwjpzqqpw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/giepbizbj.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/ggwmcludg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/giyrigbpl.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gwahpuucs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gyhtnynyv.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gzrsebwhf.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gnlvlvtvx.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gefqbqfwz.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gqoqvuvoa.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/guqocsdxm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gduwshmia.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghxarmatu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gtudjcaya.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxmaysmvi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gjybutszk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggfhkudjk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gsbqbwmny.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gttkrxory.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gfeppohvx.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gchrrsugb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/guhnfzipn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gidlgipyq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmbfvvfyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gklgcbipy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpemgpbik.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ghixujpqh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gszonozhq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmpdtntvt.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gcpkhupch.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gcrvuqgqr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gulbuejtu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gycqnazdk.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gsslsxeiy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gcrqjrgge.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gmrhnoqpl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gkzwptlvn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gqmpzommq.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gygqtwtin.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gnkiutxlr.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/ghdkweesp.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggvazvtfw.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gmjdafamy.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gvncovyeq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/guonqlnan.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gbouhkjxv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gkmdvfqab.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gnggvonuz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gqpohfxsl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjyuqeklq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gtbbxfoqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gnzqkgten.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gvfwzsqqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/goledwutg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gserenbsk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gkmvtadan.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/goymltymi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtutjxond.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gmeqipcya.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdqarlzkx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ggdtuvnky.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gdpqoftos.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gusditeuv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gptonophm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gkfloclni.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/grucorkmw.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gkzvfozfk.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ghxginyrs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glqofslbt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gucuvhsyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gyfcljqgh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gqmruwlhu.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gghosmoep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdhrdfgwi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/glzybxgfg.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gegqxqaqb.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gxgdkogdo.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gwwatfawg.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gnurmgozw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gfrchjfrs.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gaquhcsyt.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gxcysqsdk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gsihthftz.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gyyouuhun.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/guvylryte.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gmwwgblzg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gahaxiskj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtutxzcoh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gekwgawif.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gmkjippdb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gngiwpvqs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gjikcbhrk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gqdhththb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gkdoaytod.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gqdgavhlu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/grvxqfwfu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gbpwaohbe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gyswjwmxy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gwigfpdum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gdmoebpnj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gaicjrqzq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gygnswcli.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gatczyqob.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gxezvnmkv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gapojjojw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gyxfodaeh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gulcgbiuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gymdudxcm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvarwbmhm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gvgnhuest.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gonacahef.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gavqljpgv.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gxxsraxga.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gncfkqxry.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gnismoors.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/geljpvwxw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gkaspjvru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gpaxbsdbc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzujvpma.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gxvqdmxxs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/grpyzeurb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gzpkybren.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxtisftuq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gbfbhaxxj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gpdsuheng.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gedmuidvw.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gccokfkhb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/glppsbyqb.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gsmfczowt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gidiyijje.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gydyqenwb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkuopshdj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grdkntary.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfvygjxlc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjywbzvgg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gdqetkrbm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmorvjvpi.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gnifvzgfu.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gzhxksbqt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gfcedybaq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gmdgjymjq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gabemjcng.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gvhaxjxth.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxqhimwzq.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gmqigvwfv.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/ghudqokbd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gopwgmgha.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmfqura.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gctuxgcne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gvjrzjdzs.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gxvtofbay.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/geubadehr.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/ghwsftrsm.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghrninbap.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gsaituhst.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gfrtozmiw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/ggncxyken.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grrvkheow.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/groxfydlh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggewgjrpm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gxrbjwhph.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gwdvceomq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/ghdurniwd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gsrlrogjf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gsykdsqhy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gobymzpgf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/guxavrlvx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gneazrqqt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gdavjdygo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gjtagdnpx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/ginxcfybf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwpsziuhi.sHtML


<!-- 参考信息 -->