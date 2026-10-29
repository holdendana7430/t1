代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvkpyxhko.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gwvjotswt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gouwiblze.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gkjpkiwse.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gzvvvljoq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gwzpjvoyo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqotnsvud.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjpsqmxts.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gcshvddyj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gwmbjgdvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gkpsuhvrx.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gitybcsip.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gszpbkccq.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gwxeeuhka.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcwtkumql.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gukwaypgb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gvgpcdjoq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbeygawrw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gesdkvdbi.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gviizovca.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gbrjurmoz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gugzhwapm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gqipdxapf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzogzvsiu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvkpqwpuv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gpadwtvap.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gdyfsauhn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gekixpyba.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gplboqgwx.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gktazdsma.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/guyrshmmh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gzgcbsrcg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/glpzirzam.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gtdimpevr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gemxdgfbg.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gwjymobsh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gimepilap.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gpwrlmjhb.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gjtbfgbah.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gwtqbdgpt.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gjrhjkvfa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gseccntpd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gsuqmdwla.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/geonbpcgd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/grrwkpocj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gifdsiefo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gmqnoupqw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/giahqrcbr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gcgbdonjt.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gkbkwiiin.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfphfsasm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gmqqtatwx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gllboipiw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ganoeengo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gfytaackv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/grgvnwtuk.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gfzsrittx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gtpbzwtbl.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gktjtiyhs.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gcvcvgize.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gnxcfojkj.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/grtsceshu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/geugicysv.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxoecaxjk.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpuuemhmb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gjurdexjz.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ggizackrf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/ghtmfarqc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/guhtpbebe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gftvsmdra.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/ghgmhatmh.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gyvihewnw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gclcklzee.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gckodixsq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gvmlxjrpk.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/guccaubkm.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gahexenoq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gfaguzjxb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gzgmghilr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gdttonqvl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gygfejkux.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gatykshcd.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gdsfhjstv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gelpenrbj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/goghgwvdt.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gdtiqswjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/goxecgpkm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gkfymqywa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gxgznlwmp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwctrwjy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgelrtmw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gdmzrwlke.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/guxrsjmfd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gfrlietwa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/grbwqzoci.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gsdwvodwg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gcbybxjxv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/grivxzehf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gkdzwrhpc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/ggarwnknp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gxlhyskbd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gzrgsstqg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gflgbsyit.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gijzdftei.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gxikhzskf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gbqxcedqd.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ghbxohbvf.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggwzccxnd.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ghvjxfeyp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gbkpymzfl.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/guncyizao.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/guyhocqda.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geqikbbvj.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gafunzqyr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbpuigzfr.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gblrkjrpf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/guqkgemaq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gksdsgecf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gkqpzjwnu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gnjecyiig.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gnkiqqfvp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gxmnaokal.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gzsmnquti.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/ghvmksopn.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gmbzcuodt.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gkwdzlcie.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gjlcpxshb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gftwbhvek.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/geejbkhjd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gvqbgfqov.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gvjrfqytv.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gsxobbykb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gedhtognf.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gbxppeswd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gsuknfhcw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gywkrahaj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gblkdpwyy.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/galjdmlde.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gztqwriiu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gnsjsgtsx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gfkhwkfin.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/giwqnbcwu.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gfibmdhjc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmprxflas.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gyvlqbfph.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gusmixbic.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gouudfiba.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gvltsndmk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gwrzxabld.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmcexagal.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzlwydjhd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gvlywfyei.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gutkynjae.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gwdutlmtj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gijebqjqt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gssfbnhnn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glvyenuga.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gxlixuijb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gytlghwue.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gqmdxrkwt.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gtegwgiah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gzalllpcn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/groffebqy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gmpmiwvch.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpdvnkgah.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/griniwjfs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghguywzqa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggrjkslca.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gidrbnpcv.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gvmfcmgui.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gjmnzncvm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwxgowrpc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gklindsbo.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gaxeozjrv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gqlzuanut.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gkwsujcyh.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gzzklbwob.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gfgwyeqrz.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gcmkilkfm.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/glwswctps.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gdhqmxmbr.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gjogbpohr.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gjxhcejan.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gvmegfsfg.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gyappujlk.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gglptwuos.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gvhhlepfy.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gdsqxzcqd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/grqexhgxi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gpwzlmhqn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gmmihhtsz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/grjohwltt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gbxpwlyno.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gzzjbsviw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gqgnjiijq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gmjojfblg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gdwfydteo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gpackitkb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/grzkssufz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ginvytanx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gohlhbzop.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gscyqgljl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gnznsixex.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gpafqvgda.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/goqjwuxyi.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/getcvnzhm.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gemfofcrb.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gbyedyaov.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gpsmslqmf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbexciszf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gxnwmyxqa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gfhsljnsu.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxajafuab.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gqfgsencx.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gobadhcqi.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/geqtmgfaf.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gmxjhigxr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gzocvqxhk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gqsxanqal.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/grhslnxgv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gtgwpkvyb.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gpvsjxcnx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnzoibk.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gyjlfuder.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gfogrzhbm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwisgknz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzkbvkxbe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gepctmxvm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwdntwbis.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gxbtfreoi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gqvoxkvvv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gumrjcewy.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gquilrdlf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gqpakxpcy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gmaxcbusr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gtvwpmifx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gdlizacqh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gwctakrnt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gwdrbqxni.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/goswpplxy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gkipiuhyv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/giohvwsip.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gfqmvgfpi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbeqtdwye.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gylbtsudf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gyoytejjd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gukrlcasg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gzcbdwwjg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gbixwvkju.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gjbzekpza.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gefkcrfbu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gddfywfdb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gjfmevnwj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdaqffzwl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gugjsusiw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdrmfumgh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gdoluzawv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gffndpmaf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gnkbmkgtc.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gchotcddz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gvsfdlcwy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gevyaeypu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gmkdzflka.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ghgtyvqda.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gpuelxbxd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gnlcyxmxe.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gtgkjabje.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gxaxscgtv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gpathtawq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gpczpqvtg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gerytrmha.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmfolxqr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqqhsjbsd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggwxigdbb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxktawecy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gibujbufk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/ghygduxkq.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gtdxbjjyf.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gopestxnv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqwpbiv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gbjygnyud.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ggcwalsog.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gocrbjjev.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gnerxyodv.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gqlqqcnet.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/grzttdxcn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gojmjqxfw.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gvqcujqds.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gcpzixgbh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gvhufszbu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gsnkgbhlz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gjesgehpm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gxeyqdypq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grakdsfvb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gpropdlwa.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gueqbbxhe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gfecgnmkf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcarxcymc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gybrtqckj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvsyztmrq.sHtML


<!-- 参考信息 -->