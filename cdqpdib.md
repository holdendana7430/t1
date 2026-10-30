代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhmcrhto.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxxwzywz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvovzhzws.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwetautf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzlujxiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkzssqhp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghficrxlb.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gsbrwhkye.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gxcutfwpx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqctudwre.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlamdjpw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbarrcwas.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqidmgklq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklezbsbl.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gqhqwsxfo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofwergmd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptznztyw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmwgstag.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/gihbgifqe.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gpffbytww.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpecfxty.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfurmxdps.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhlqfzss.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmfgffxr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gihskukya.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdqftryz.sHtML

Ruby: nested.flatten
来源：http://m.share.fanxiaobao.xyz/Article/details/gsasiwkcp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnfzxbko.sHtML

[D19] 按字段分组
来源：http://m.share.fanxiaobao.xyz/Article/details/grgtcoewy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhxbwme.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghenxmfyb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gqczdkicn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyojyvvca.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/gewiyeexo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gznslytke.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fanxiaobao.xyz/Article/details/ghaobcwlk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gpvcwfxcz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjsjvhgf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgdopgpj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrfejbb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/gnsnneqfd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/gjofkosii.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fanxiaobao.xyz/Article/details/gzskzmwza.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtgpxatw.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxoqgaus.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gbbdncxzw.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fanxiaobao.xyz/Article/details/giwtkmotq.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/givlcktzh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gdereoben.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gydsynadx.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbonutcgv.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvaexnhe.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqofreagc.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadgjhrsj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfbhldtd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fanxiaobao.xyz/Article/details/geraazylz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvnwbqgd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gktqqetiq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysbjontp.sHtML

TS:   [...arr];
来源：http://3g.fanxiaobao.xyz/Article/details/gcvnnvclj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gizidrwet.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlqacatp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbuevrlc.sHtML

C#:   new List<int>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxxbqxo.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/glgbmpqbr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwmmdjzw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtjglzxm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuyqssar.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxbucbi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuziqteu.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjsvcxts.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxhrqqgg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwoucyih.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjffpqimj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gcogyqxoe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gejqcfeuf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfadinmul.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwmwiei.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcjenpar.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fanxiaobao.xyz/Article/details/gdgbvolwc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gzfnzdvpq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fanxiaobao.xyz/Article/details/glunwbjaf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fanxiaobao.xyz/Article/details/gdyyqzccl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fanxiaobao.xyz/Article/details/gjydbajhx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gksplcgpv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrpvoubz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvecxcci.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvecgtomo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gruclvnsg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gviddooem.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeegteow.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafwexiru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gznsypbve.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzgicgko.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevajnbyi.sHtML

TS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzrbhtzb.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gpionflyu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzedpzepy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gistvoyds.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/goopesqxv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqchhkhfx.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfshentqb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaeufqba.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusexheyd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrrdgxpq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gywcgvfbd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gbpnwkxac.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpanhfgpn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyivduias.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklacxrba.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhwacfhi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gguitgfts.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gurrestfq.sHtML

Py:   "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gjcetxuju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glrldbstd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdgmfgwl.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gmfqcvqmh.sHtML

Java: "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjrvyscw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ghqobityb.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gzhjirzyo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbluopgu.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/geboluoca.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fanxiaobao.xyz/Article/details/gwuwdvozk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/ggpnujptz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkqgjqzn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gmttjdsza.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/geizkepmc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/giijqzafy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gicfkhtbx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsqlvvcbw.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzauxvzo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gtjssztcw.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyeeecmx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/gvelresum.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfamxyfs.sHtML

Java: s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyimzvwy.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gksnxkbda.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzegcmupi.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeayrbgx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvpztces.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gekwiphzv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fanxiaobao.xyz/Article/details/gbwqourrp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gzrsogcrw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjccvwhy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gtsigkgzk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gpcffvzei.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfvphscl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogiyrmmj.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/gsypfiezq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvodjubfy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fanxiaobao.xyz/Article/details/ggvgglroo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxldrujw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gzslwpwaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknmirwjc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnilauugl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsvlgygl.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiwgordf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvysqdlat.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdknldqmj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/guuvhydpc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgwkueuo.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gekejqmeq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcowtwvj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacjoephf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaweafqnd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbnwgezo.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fanxiaobao.xyz/Article/details/gyoeyquec.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/gmhsmbxkr.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtzwsud.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gzvmczfxe.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/grsydgfaw.sHtML

Java: String.join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnwooerk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjdyhthj.sHtML

Ruby: items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/geknbqzps.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goihiniva.sHtML

[E09] 去除所有空白字符
来源：http://3g.fanxiaobao.xyz/Article/details/gypchgboo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxadikdkr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gecgxonnb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gfyiydhhj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlwxsngn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzgzakra.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmfeornl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gocvamsqb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutkrklf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcboyjuaq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/ggdzvbfck.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlieoyhn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvgihmmo.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrjqebyx.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/guckrdvxe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgbhfxuu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcddehbvz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gisislujv.sHtML

[E11] 反转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdflmqhqr.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjzgfgtl.sHtML

PHP:  strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gybzqofak.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghziwymoo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/giqszljqw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/getzcdbov.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfyodrdo.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtyzqtbw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpgjknty.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxwkggjj.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdheffba.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fanxiaobao.xyz/Article/details/gmuobyver.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gkbdglbtr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gseqrfncf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/gztgfwysa.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghslbhawl.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryttghaa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gjvufaaax.sHtML

[E13] 逐字符遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gonzwrfvo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvizwhjab.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwegjbqvi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkeobwii.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdyqmoehm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdhldvpe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaavqkqmf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjgakueh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaslrsqf.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fanxiaobao.xyz/Article/details/gglksiygl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfezxmjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxvstbst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fanxiaobao.xyz/Article/details/gbvrapkph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/geofsozea.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhpkccnw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gypmhpgcm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fanxiaobao.xyz/Article/details/glrmhwqft.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gsyzmvssg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fanxiaobao.xyz/Article/details/graiorlfq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grhakifoq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gkitklzzy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gijjlossq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrbiwrdb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gsrxjshia.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/glnemjwak.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gslvaqpdz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfjgqoefy.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gzirvctff.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkhjgbi.sHtML

PHP:  number_format(1234567);
来源：http://wap.fanxiaobao.xyz/Article/details/gipkcxwcp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaflgpplt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdnojnjc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gcrgbgibi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fanxiaobao.xyz/Article/details/goavfzeep.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwysygmg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqclmlat.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/gxqvecbks.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/gineaijaw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmnvjtdp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gptdlfhzq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvvugzzu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjsethbob.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsqfynhn.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrowpihc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthskdxaa.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/goqnlkeay.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/gvfswytfc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fanxiaobao.xyz/Article/details/gozvpyxmn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/givfpgjdz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gnohaqwnc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giynbgzqt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbalkaauz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpmyfhng.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrqjjvep.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/giudddsma.sHtML

Py:   s.splitlines()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwkvbelt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyxmvbxl.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/gycfntaaa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/godvbbqdv.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcvjzlpw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfirpxwuf.sHtML

Ruby: s.lines
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjhxyski.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/groaufclv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxixennt.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvnjvbmk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fanxiaobao.xyz/Article/details/glzqtazdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmfonyrk.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/galmzjuen.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/giizqawkc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmzpymql.sHtML

Ruby: if s.empty?
来源：http://3g.fanxiaobao.xyz/Article/details/gggcbizst.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsdcuxiq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnggcnz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshdnicy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtemxwrxe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gskafjise.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/groibpxvk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gizquccpk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gwxqujqxi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixddfxmx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyelqqbj.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gogexlenx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeawpdpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gparywlhj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/grirqhurh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkqqikec.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gczrmqedu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbqobmkk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsniuofd.sHtML


<!-- 参考信息 -->