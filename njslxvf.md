代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gevmotjnp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdufsaqao.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gylspuvlh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/givyhihla.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gwwevdxwv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gdydpjxpv.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gmhqqmygj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyuopvupx.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gswcfnlvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gntyftgdc.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/ghbqrsdnc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gatujfgjg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gkzmavsqu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gyorxknet.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gjomwuhbq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gjvktzqwf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gracmycwq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gtbewwwvy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gaquwfgxh.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/grwmfmaia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gexunxtnc.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gxvobgenv.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gxlogxnno.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gbsaneunv.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gzpuspdqf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gutnnaxql.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gzbqwmsdu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/ginbhkfpj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/ghphsxadr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gcykcendd.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/guwxpcthg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ggferntfw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gdpljqcet.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gowvpdrmc.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gaffnfmqy.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gouzhartf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgfdqyr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gsolkhmel.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gzrfyibov.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gbtpgtpcs.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gguparbwr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/ghumxpdly.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gehbbxumu.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gsfjcndwk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gxtxdxkii.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/guhkiwtkn.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gricisjnt.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfmmrbhkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwvblpxcc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqsconpur.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gmzylwkut.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/ghugjtgma.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvfhnrtmb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gtzgmdmda.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gvetoyitz.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gzrfkulpb.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gqyhmkoqa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/guruupbwj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gmicadcyz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsfaiueb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gcjumqnso.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gpojqvyfn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/glmeichbc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfouxltsu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpuyfcjsh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gkypqwvpo.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gxsvapndt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gpryeicqi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gehpssucz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/ghblftndb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gxthhsiyq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gttohdcpm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gaanbflie.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/giztoefay.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/grlmdsxyv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gryyjerxd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gxhzwryta.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gmhqkerjc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gvjlcivzb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gyhilbpuq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/goeolmjhh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gjivborih.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gbjctdbvo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzyekxxht.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/glhdmoidn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gqwkdyyom.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdscfpo.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbartzije.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gfexdkhmj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gaxucgmgk.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gebbenxra.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnoaznptm.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gwtlxanzc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjoeiijzj.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gvcsksbtm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gticlgfdp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnwusbvgt.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gflucxfxg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkcwsnvsn.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdxjdnzbx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/grrmxpldu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gxrrbdmen.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gyhyzfqgi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gijntwxmk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gccxqmlfg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gsorakjnm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gwpajoclb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpyymvqte.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gbkpdtgky.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gwmywcoxo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gcrjcapak.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gvsefhvry.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gsgicoloq.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbbbrcfrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gfunekfjr.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/guhgbotrg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gduuybfdy.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gtfalsvif.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/ghnepgvgv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/glfjuypcm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ggugisplv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gaezfouaz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gjjmikrwj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gcginlnkc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/goscldttq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gccadhhig.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gdbozbflm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gomyhgdll.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gzkkknfgl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gwowxwjts.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtzeulbsp.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gdgffoiub.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gkbpjofaa.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gfvsxzpnk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gjkzzgcfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gthownxqv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/giheweywo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/glcrhfqeq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/glzphxjio.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gueydktgg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnwdmqkwb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gqnfuowma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gzggtwurj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtxmbbaj.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gwmqqdbjo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gwwyhgxme.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gwrfdaeck.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvjegicry.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gimfsfwpw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxjtsukuc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gybipxymf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/goyzmvstf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfenuxxib.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gcenrbltd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gutvqkpot.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gtefcdpsj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/garkxahyt.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gnzorlinp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gypfmliqp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gltwnrpvw.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gsjvcfxfz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gvwfimbnr.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gfeynmsog.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gplcjxtgx.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gisswprwk.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ghaozqkmh.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gcjuvkcou.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gybadluta.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gkkdgpody.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gjakmioow.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gpxolfwar.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gsgbmewwq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gfyibrazk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gwwcbiksd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ggxeahcsf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/getkhdbmq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/giebjvnlu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/giexljudo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/ghghkydsq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gcnebsjta.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gjqeqdpfa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjkygsnht.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gqpzfybrn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/grwafatfm.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/glvobevbd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gveqwpylf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gitkjzleu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/glmbusoul.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gtlioniuk.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/ggnbgzwpm.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gddwpzgih.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gzimnuppy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmowxdgly.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/glwohexbb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/ghyigtxiw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gulcgtjyt.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/ghofqujcu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/goqtozsvy.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gbyliamcz.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/ggozmbsjv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gpfsyizzq.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gqvjcofks.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gloluhtkm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gswnduvgx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gpuznowgz.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gmbepebnj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/glxqtphvl.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gchiwpfxd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gsnhcncia.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/ggrfiujvf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gjplzammf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gbmudvwsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gjlaqktjk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gtowqdhcx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gqgscymor.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gylxkmasi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/givirwwqk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gtbpspuvd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gugelyjsu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gkznowika.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gkutjinbq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/galfxzqbl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gynidlumt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gdfszojcv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gcaiazeuu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gbmoeoxdd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gpjjaemlb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/grtqxcusa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gfbollack.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gyrelohcl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gjaelqune.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gilostclm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/guhsfqxii.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gtmevjxdt.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghvhioxnq.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/genozpdfg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gyksadzdo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gaxhwokbg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gdyqqlcge.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gdjhecphc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/glechaqjq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/glyjpsila.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gdmdohejc.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gclfzkzxh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/guiflqcwh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyxgltctt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxbcstcta.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gsknxoazj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpugxovzi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxonmzdol.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gmxorymnm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gdmfspltc.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gywdnuzwo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/ghfgefoup.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gqagioptt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gnwlekaot.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gioqbytna.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gvlyaoali.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghshwafwl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gdsxqbnxd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/ghmganbay.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gxlhufgui.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gkfnvqwxh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gauzwawtk.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gjcqvvnny.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gdafyoyjz.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gudybpdxk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gsronbzdj.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/grlnkgqof.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/guakyeklc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gjafskdzg.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gohmwlcyf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gtekyxpun.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gwburaovg.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gwpqjelux.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gtauzhcyv.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gkrkhmsds.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gahauegzp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/guwulkmgj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gdhnzibvz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmcidddmy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjolhwqln.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbvxusrpp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpnakaexs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gheugxcal.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/glzpvxgob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glbinmlhl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grsqzyyzo.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gtptcbnpj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/glkdqtqez.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gmkidyogc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gclbkbwdy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqqiumole.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ggalfiwpp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gqshonwqc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gfkvlfcfx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gvtxygytb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggfusmbqz.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gotmznhdo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gckdyrodl.sHtML


<!-- 参考信息 -->