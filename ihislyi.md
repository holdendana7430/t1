代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gsllcnbzq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gclibkvgl.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gbdshjldi.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gwirolzoy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gnxlyvtin.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gknuhdpqx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/georyyfvw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gboaqzoks.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gzkzpmvsz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gdqhblkka.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gddmdfzsz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ggedeytoo.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/ggvdcebzd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gvzsuamfj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gwaorxpcy.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/ghhgxhhzj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gdlojguad.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gxmrutgpc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/geifeizrg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gttdxewnx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/grwpopuqb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdeoumfgg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gcqlpsfbc.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/grneyegni.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gfgrxfwpe.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/ggviobkxa.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gylpwdjsx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gpbppyfxm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgqrqaai.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gzdrqhzta.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtfqnwxkg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gqxdphnxf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/ghttuyhyn.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gcrdurdxe.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gjohnwymz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gkmzjjzzu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gajokhrmd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gowrftptf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gjcbfctyl.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/guosghqgm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gwaxhtxcg.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/grdnijalh.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gcevorynd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gxnhmmdxk.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gfbdedpos.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gtucejqlz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsipcsj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gjeqnceip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gjlyhuats.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gbnyoxynn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gltugrojb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gaqzwmgav.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gyjsxrpde.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gnzsudtox.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gybmwovmj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/grvchyybx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gxcffaogr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gwjneldkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gdldmfbvs.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gsdetiopo.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gwyznhkyf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gotvbfqrh.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gvtnzqnfp.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gkucdzgrt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gurmbdtkr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gsowotwju.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwcslqhff.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gfpdsjtwb.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gavbppzyl.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gdmmoumhy.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/ghtpncvit.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gajnxjebv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/glpfbdykl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gphajnyuu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gpgiqjuco.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gemfdjylp.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gsurrmsce.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/grmyipctz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gckfnqlqw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gotrzykef.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gscfxizzz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gyrozkazz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdaociufc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gpheygrzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/glxmsqigf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/glxmikbau.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gftetigtg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/grwuokfuj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtllszst.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gxyasbkin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gwgmvewnu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gtgxhhsvy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gocuxtvao.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdxophxrq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gouyhdwaz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gkpwvwwbs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gzoswhxdz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gtaipmkcq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gornywrip.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/ggkvkdcua.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gnstyfnze.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gjbepduwc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gyxdgmepp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/glczbhuno.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gaoubqxin.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gskmezcld.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdizzltov.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gmwixsayi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gutdkpcez.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcpdifnqc.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gciplzscr.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gauthhpcr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gdpmikdcz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gdqgjktey.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gfvocivdw.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gysftdrjj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gegqkxttd.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gbzpglgxu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghakhulbe.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ggqcwxcza.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gbildgkfx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/goisnjlrb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gwpffpflb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/grmuvpwdy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gfzsfumnx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/grwrjvdzg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gasoauxqb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glrxkaqtk.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gpkywtclz.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwebxitfc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gdebkjols.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnsdgdbqb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gvohelgga.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwikvmscm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gntkqstck.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gqvkcvwjn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gzxjajidf.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gpkrfquoj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/glgsutuat.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gonvuvnel.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/giqjkeqqv.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfxwasaez.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gswxispga.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gzclgqacf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gnaerwwrq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/grbxiuwhv.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gaihynihm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/ghcnwthae.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/ggwztvaoe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gvjatksxa.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/glaxrgzos.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gnxcodpoe.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gwjlzopfr.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghuzjwvxz.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gxkhyxuzn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gijqmtrzz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gwyntmtcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gdzaslxbd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gvhqpcxim.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gncmcwejk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/glmlzjife.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gniqlhpju.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gmivczarr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/glhncigoh.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gxzbljhvx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gidifpwtq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gvolrileu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjsipzppy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzaamrtxc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gygmcxeln.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gizloigsn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gltxbzift.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/govokyihp.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gwmxhizbq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/giulvpuik.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gzvbyhcca.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gsqqihthd.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gehbeumeh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gnvgxujdi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcshwnopm.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gppmtduvg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gvhpjnuok.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gojffxuht.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/ghxscmhot.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gfalqtafd.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gghfhgqly.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/giknhqeso.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gmbzrfyyg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gisudbfjw.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghytxnouo.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gvzgidtnq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gytbwilpe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gtqtywlyn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/govljtepl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxpdiqjjh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gauzzclrc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gakyssrqg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gkpwdqbia.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gtdwzrfjx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gkilsvomb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gxjgqsoht.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gsfsizbvq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gnfpyksce.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/guetxqfyg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gnhptahos.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gtsqikome.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gzfoqtybo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbwfshgsv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gmvvqnfpj.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gnxeflpan.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gebmzjvju.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gxkehmqlk.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwvutjdyg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gyheeeoho.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/grdsttibg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/ggtkvqiuo.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gyrczgxnf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ghxkhsghc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gpzozzjln.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gkqfxzggc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/glorcdqyw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gxqzxgnwd.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gankdmcom.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gzckrrlbo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/ginytlkhi.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gqldjfozt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gnemtybcg.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/ghpazvbng.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gtyrcyeuh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwuvjnex.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/glozzcnis.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ggvjuloev.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gyglhwyad.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gopbsldib.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gswaekfjr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gjegarpnh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gwclrumuj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gixhnfzor.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gfvnicdkw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gefszhwtb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gjtrilonv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzizjnzv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gvsxzpoti.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfaixvilq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/ghrqffwij.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ggrlzarlg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gdlugproz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gmhxsvsge.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gmefpzcgy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gxahfhbpe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gvmdgwoap.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/guprvtlwi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gcmybfthz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gidrvfqvb.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gnmfalwvp.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gbeespwgs.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gvvhkqlvg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfvxzbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gbedwkvvd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gfsdblvqw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gynpbyjgq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gsgwvybjx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gfiuwkrbd.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gjwoxxush.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gaoibjobw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gnfkyglqz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gqviwcimc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gviiuxhkq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/grfjjaxti.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gmrynxlgn.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gyghpsffi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gvnkmntgl.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/ggxkuswan.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gxrmxltyj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gjfealjhw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkxklzasv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gxryzkzom.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gjbpwrokt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gyjonoart.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gwhtjqpbg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gcrpynfzv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gqbarejgp.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gafnrbhjt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghpyltkhc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gsjjoonbd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ghmrohhfe.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/grnmhdneb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjnnlpcvz.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gkarnqcib.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gnpxdqthj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gsgtxkwkl.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gxrxslcob.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gtnmbmrpv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/glkuoscsj.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gngevftpo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtukgstxd.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gddyxebfu.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gygsxxici.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gsrjpwtvl.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gnzklhiir.sHtML


<!-- 参考信息 -->