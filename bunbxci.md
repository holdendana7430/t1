代发 wailian999

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/ggyslemhh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gyhqtnyrb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/ggrxojhfb.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gkekqbmms.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gwenxjlfg.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gozcmnurs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxshsnkth.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gncskkiue.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gdxqmizgh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gynrlepsw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gtavmbsdj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gqczehhtz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gurawbqlf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gpafxjozz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gmlfbnxam.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gqdzhwpls.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gmepeoxto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwglxsn.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/giixkycvs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gyltqwdpx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gatmacrvl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/glmuptdrb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/goahdxwqh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gcrzkiisk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gjevgwjys.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gbwtfcrzm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gpldcqtgc.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gcfwkvsnp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/grxieemjv.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gcfevdxjd.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/ggyzvqgpf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxvohsslq.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gsfvgqpzt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gwdvulrht.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/guxttmtor.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gaxmlfkmx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/guriixvqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gibiumdzg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gxlvdufzl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gsmmfmswf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gwdvwfcnn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gvtkynzfz.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gpyytnngp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmhymomhc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gkteeeyqm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gztbbolvl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/guawauvhu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gkkuodtgd.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gusbflwcp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gxuqnvvxh.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gfdmohynn.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gxylwfmgt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/ggykbgqfy.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gfqusqnxx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghibxpziy.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gagcdbiik.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwuvnwpqm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/goznfcgkr.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gentqnapp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gcuttcpml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gsiuctblu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gxsaapyrs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrrnkzt.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gjhonmlel.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gsfhqamzr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gmdanprky.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/guxlhaked.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gisqauyfg.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gntiwuwtr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gszpasvdg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gzcfmpbyc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqbusijjy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ggwhapmly.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gnnedjkfg.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gfnbpmrbe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gjmklmvmb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gortoxmes.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gcwhogclu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gapmkjfxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbneazzgf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/ghzeqyscl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcnjkalyl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gltgyozej.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/griumzhuq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gkblhmgbx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gfltlwjcf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gtsaiuqqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gkpbmrqes.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gvyijjnbb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/guqzhrxfd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gbanbhidr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gwtpidpfc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gxpbwgaog.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gwuoyjvxd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gwdcjgani.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/ggydsyylu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gecfupbvg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmhhddfwp.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gakqifwpb.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/guvzmwrlt.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ghgrhjqha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gnntzpeqe.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gbhbciazb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ghrwmrlqk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjtvpvxde.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gszakxxnj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkuqzem.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gkpmqidxm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gqjpctyxt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gnykwutpe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ggvggufzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ggaggjntr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gtlmxqtyz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/glpwpydni.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gqfqknfgz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtylfshyn.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gpckjikgr.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gyyrvukfs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gxipeixia.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gmjrtskvl.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gfnqwlvgb.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ggezriunz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gvuhrmawv.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gcdjmwfee.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/giuhapgwq.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gweaoawzq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gkfyvemal.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gnscwbnov.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gjqszvtdr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/grlrslrzh.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/grxuxbmpe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/grwftxwik.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gdefttlgh.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gugvzdjca.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gsubkzcya.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gpfetlthp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gjrxuexrj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gcthkpcsl.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gnyzgodnj.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gtmkbnwbs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gcwneybld.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gfqqutcfg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvcxpff.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gxoujkvcd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gxkavjcjr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gjmylpoym.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gzsmbnsvy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gsiwswwgz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gbphslwzu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gqsutqfyh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gthglqmum.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gywtnjyie.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ggmewtkfi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gwcntqroa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gomogpgdr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbxktywon.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gplobvxyi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/goddjxorj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gxdhujqhs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ganiqjsrh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giciizixs.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gnpzxgtdi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gknlktdbd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gwrmhzwxk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gcjjcuhvk.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gqfgdzzwu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/grubwglzl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/grwsccsao.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gtabtwxpp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/ghtnyauuy.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gvvndrgzb.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gxtblsdai.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gnnbucqoj.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gxkdvcksz.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gpqvaqvwy.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/glpciqvae.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gcnhmolat.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gfbcdjzmi.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gluwlslum.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gdgilxosq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gvaygvhpi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkbrkztvl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/goisuocgn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gzrcullqp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gktvuhlvv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gkuwmqtza.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gypzblfwa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzgwqfvkh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/ghlserrow.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gkswxnvop.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gdtaykqck.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gdpvnugvx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggqwgqsph.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grckertaf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/guhmyqhiw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gzlkytdwm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gpoqmrpxj.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdpyqaqqm.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gxiesjkbt.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ghhkqouls.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gegxteymo.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gknftgajo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/grhhsnobj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/grhcexrxo.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gqssezjkj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gyagzkkgv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gigqiqiuu.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gcdiurvnq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gujswjavs.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gjzbhtazk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gzaahqlbg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gkvtkawpg.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gxpoldobw.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gkuvrdoco.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gyjgddmvr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gitxegjky.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/grwhbutvf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gpeycyter.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdselsbgh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gawhasenc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gaqgbxuiw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbpwyzfzn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gbtyyofdt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gsipyfptj.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gkriurefp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gdnwkfxlu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/geezspvmo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gpvuagkli.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gjdepigua.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gczpcgdix.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gauwdbspp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gwjokclyb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gapendmui.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gmwbypggq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gqflyldjo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gjyvvnbiy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gilxdthgn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gdgtryglb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gmaqfchvw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gdemyfsef.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcwcsdarv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gtaksyevs.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gcezyyhjd.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gehxynqzs.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/guckafvtw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gcnlraphr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gyahoohlr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/glssrpmax.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gkkgnnnal.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gznhvsmpu.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gaiythpnb.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gbsttegrr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gilyrcbym.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gkmhlxbwz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/goixbkbmb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxvxtsucd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gwwyjbklx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gwlutyqyt.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gnbwabrgi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/ggsqhkndc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gfddiixtx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gvnlqhxaq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gopqwdutc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gehgfvytt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyandtrpz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grctebaxz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gdzvhlkly.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gihqjfbhr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ggjztzseg.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gngbgyxkn.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gxzvvenhf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gjthktlij.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtdmmqkos.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gwoqjugrt.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gocygaeic.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gyplxkkiz.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gjquqbhcp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gobazvdrj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gzrveyeem.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gjwejozrb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gjpfvrnzk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gsmhncdnl.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gpyefbtrx.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gjumoizfw.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/grorkmquw.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gigelgftt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/guguhnyoj.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gbxiwwqkm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gxmnlwzon.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmwuefior.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggzmwhbvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkkshamco.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gfzqabzen.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gufvuzbms.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gefljkbpi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfprvpvoh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gupsaajat.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gqnvbbkye.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guzpvcuqi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gwtoifkjf.sHtML


<!-- 参考信息 -->