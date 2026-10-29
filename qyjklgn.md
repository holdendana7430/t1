代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gfvhrdsua.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gavjecuat.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmyzgwyny.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gqptvmydg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gfbckplqo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gguyqbwia.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/geipufzue.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gqtkjbmai.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gqallsush.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gpgnpsxfp.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gsgozuwhv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gawuwojoj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gbwbibpsh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gulsgqoax.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmhlwvecx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmkzlayeu.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzokkfkxp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbachjjob.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gqynzwncy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/groxnyjet.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gzuyqwukp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gevsnneuu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gyrukaunb.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gwjveeuhq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gwzvzqiyg.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gpxapdnuq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/ganiqcxde.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gkgumdycn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggeixotgm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfmebpbbl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gmfklsnwl.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/ghptfkuvh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/ghdgjrkwx.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gszuzvxlw.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gxcjvrqnw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/guehgeqfy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/grzokrojy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpechpwg.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gmjfghhrr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gtffbvuhv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzxpehqhd.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gclejipqa.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gllyqyqpc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/ghltrmrvi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gdvorvthx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ggpfglsdt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gddkqlejj.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gjqwnmbjm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gtxdruamk.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gxmenpuyi.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gcphofhxu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqapclpij.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gdlnvcmxo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gmzcnbxeg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gbcniiaak.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/ghjjzxkil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gyyfkcdkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gpaspikcg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/ggjggseke.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gtbctpbgs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gyzftjuqd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/grwsjrlwi.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gagrqyovy.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gjvywxitl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gqulttxnf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ggxgslhcd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gelvfclpr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gnxnrepaf.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gzjqfxdpi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gvortlyqu.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gvrzgcckn.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gtmjjrfeg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gcisikdxp.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gsxtsfcua.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gacoyqyfx.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gqlnboyor.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gshccrmpe.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gjmyeifcy.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/glyuckolu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gyulfftmf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gutpevsis.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gedeqqxwy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsbfwqsbf.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/glvgulfft.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gdszatfqy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gdhokcyon.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gmymzsctl.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gxuepibwi.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gajdjjnba.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gvumrrgkx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/ggftqyrby.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxagtodez.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gjpxrdtbt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gmmhqnvtk.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gazttwcsn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gndbjbxxw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gpsblmcpm.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gfyecdygz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gkpuodzaf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gishalxge.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gfcyonrfr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvbbyfmpn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gtaltbjbs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gpkkyzola.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/goftwgvzi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gvaypehtz.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gjytnuhbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gcouseihw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gtebwtgzy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gwedsccre.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gxnqtkwaj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gmdgizguu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gqmgzsknm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gstnpuvdp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gsflmxehi.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gffgcshrn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gcghpzmhq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/guiohsrfs.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/goxpsfeid.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gbnieedpa.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gajrcwzai.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gyskhlgvi.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gpgkdwusq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/geffgvbyk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvinwqbud.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gkwozbdcy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxkxeigo.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gowzkibvf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gafvlzuqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqzmdmfh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gnrzwtpfp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gijmoowoh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gzfqjynub.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gfhizmjsl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gbpvibrxt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gcfjnjses.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gqcabromo.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/goyfdbnqv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/grpodypek.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnoereab.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gqfzbpzpp.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gqwweqcny.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gbdqlwtbm.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gxzyeokky.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gzayodgfx.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gkohywlax.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwsncrzxu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gvefaklhi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gunenlysz.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gahjcbxna.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbuqqacef.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/ggsahqrek.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gqpagnczj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gshcbacdt.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gaeboytad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gfhndqmeb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gqbfwjcnk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gythrwkpj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gpqizvygv.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwarhkajz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gtewslkra.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/ghymbuwue.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ggznqdvyf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gmtkgyinb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwepntf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gyikczrcz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/ggtyphnyw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gmjikfgks.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gveuthncd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gdblxgnql.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gevzffeva.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glziscnqg.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gcfsprvbk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/grkpdjkpj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gcszoecjd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvusykoba.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghsgaeotc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjiqzuwrg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gkzaiyxsz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtudxjapy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gsoshjkcj.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gkhelfpbp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/glkbxpcbg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gdlyynbtg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gihqmykjl.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gkikysvuj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gwqpawlft.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gwmoszkmg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gxumcsuwe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gjifvfhrh.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gfvmmxdbz.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gayebffru.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gtcjipnjj.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gxigivtbo.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ghjwotjyy.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gnfdmfala.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gnmmmjjkz.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gqoutgvui.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gbviykezu.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/goyktznal.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gylpgsobp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcltqllvc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gptvvggox.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gybsdnfae.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gffkslrqb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gfimeuajm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gjkyjdjbj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gbrfyogxc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gsaecvbga.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gnwppyuno.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/ghbvdaxfw.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/golzrkbwm.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkokffdad.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/geozewwxf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gpwgdflvg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gqtqkkltd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gytgahrky.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjtxxfwam.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gskzrczdr.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gmbcizfao.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gcfbqfnsn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtdphbegx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gvsevcifl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gyfiyzsen.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gatsgwavc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gmhdfgzik.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gjvgzhocw.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gwtxdtwpg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gchtsxfaf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gmmnhetin.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gjuprtgzz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gnqdprumk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gppacjior.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gewdjewiw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gvgnnstmu.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/golzvepbd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gbhkiwypb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gxxkhsetb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gkiljnzvu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ghnyurpnj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gpazbtxey.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gmrzyclnr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gbvlnsttf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gktszuxch.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/geuaeejce.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gmoqcvzbl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gzapiqhip.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/grhftzfph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gvnyimijp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/geuwfbogk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/goqylqxeq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gnlbtydez.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gafqnxdpr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gzebyober.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/grqmznqkv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwsodhnxa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/goseaxumf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/goihffwgt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gbrmerhjr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gvgswfzba.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gqiwfemkf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/goqepwdjg.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gmlbdtdzr.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gdnbmftod.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gktnqwltn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gxbkgmkyq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/giishynnj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gaocectxo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gbhrishzh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gfeoazpwm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/grxhbkwqe.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gicblmyff.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gyceqaktr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdjglhwrq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gylbosyvp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gwrgvipbb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gzdjjdthm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gbxyckdlr.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gjkpowfqr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gticgxvmx.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gdoawfwgz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gwhpfisqr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gqatnfpvv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gbawflbgz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gdcbskpew.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gahwazvlj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbpbchnep.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gkjchhgox.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/grwnztaja.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gtrglihus.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/ggarhrjqr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gqpyjjvuk.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gfqmrfgvm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gplcppxgv.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gariqnqrm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gldpdornc.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gvhbawvpd.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/geiqqxmok.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gmheqrhkw.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gacvjhdym.sHtML


<!-- 参考信息 -->