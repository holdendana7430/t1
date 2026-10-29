代发 wailian999

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gmkcyumkb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gqfcuxymo.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvnkzwfkx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/ggqtamyye.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/garmrpfso.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gpqijnauo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gknidbuxw.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gvgplmhfr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gfrpdeihz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gdgdpnxbp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwgjvaqha.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gzgraoxgg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvzthiyyo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggnsrvpva.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/ganwkaqzd.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gusjjvlcc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gfmrjiczl.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gggirxqzp.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gzfrgyzmv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gkpaypaem.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gtwhhklso.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gzaeouzld.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/giibzixyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gwnrnqnpv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/glyylnfgh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gbshdkmte.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gpblqmuvi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gcfttciez.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gutvfmrbp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gcbmsivvy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gxqcqhzyc.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gaughscbv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gvrsannjh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gnpqzxncr.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/ggbrfwvcb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gplqnclxk.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gktwaybwo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gqgfxdkjc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gwsqsylyu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gzvkwapmy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gntvuuhpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gvuhiqabv.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/goysnzwmi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gedrpebxv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/glbqreqwa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/glgtyxame.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkoflftj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gncbmpkvj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gjnwhcprx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gjiqgxqaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gdaqzwtqc.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gwrdfxmmx.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gtbclnwxl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/grzztxrur.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/ggijvuogu.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gntwprzeu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gurmlpmgk.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gewjjttkw.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gghxlnpst.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gcsvdfqrh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gcsorzdzy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/guydvrxow.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gggttypun.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/glztthtep.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gsjolljjs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/glidnfnhd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gaztxwvql.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gpabapesj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/grbxcrgrx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/glkdwekpu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gapbmhybo.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/goskmxfcr.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gfsocvfgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/ggzudruyr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gmiucvejr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/geeadgikr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjdommqir.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gqeknuzkz.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gzexjptsc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gwgsmlyov.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gtbcyjaqn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gfhevybtx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmgexciki.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/genugmmiq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gsyewkzmh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghktbsylk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gflctgqpu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gipbrxbfa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/grvdiggor.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gygtvnmep.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gwqbipfat.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gywerjzco.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gkzboucea.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gbuqlhmsa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gfcbhanpv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gqtjmequo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ggkzkxhvr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gghysegtn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnglkzgkr.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gnqlzprjq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gozelbvjs.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gxivtzqve.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/garmwwajr.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gyjrfarkf.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/ghmcxrqxv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyvqvpt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/goulwlhgl.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gffgzlnfz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbsbodbpv.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/ghrlqreju.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyqdpngot.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gsbdknsfh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/glbtopigs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/goaefeigj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gzgjuhkjv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/geclqgogb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gynnsvjcv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gmiawcrki.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/getjgkfio.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gubhomweb.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/golsuxpxi.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gdypkyrsn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkclowvy.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/giinprpzk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfadoqgkc.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmrqlswnf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gzdeetvkm.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gbrxjfnvs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/giuxyylvo.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gffiwpvwy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gctytgmed.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gntnureea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtttmubkh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gfkvvkoqt.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gdkayrzbk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjffvindu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gqnqfqqlc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gxydgtypr.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gdeqowdzx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gcntvgfzk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/guyprzuuy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gxpxurvhx.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gstmiejrv.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gvvdsusvi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gqvmionfy.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gaqrcyqvk.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gsduqswfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/grmavoxqp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gyhxitovl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gomnczvvd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gwbufmnsf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/guspamlyv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/guojchzrg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/ghgjlwumn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzaxmlt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gzndpwair.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gdujxddxg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/goywmrdkc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gcvfnnmmh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gihwwpxfn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcszqajdm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnoxojsx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gjdslkrpj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gflyhteej.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqwyeijhx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gwrnmitrx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gctfszcjn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gldadfdjo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gfibctgus.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gfztartgh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gqthmypvb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gjgivampx.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gmdszluoa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gxpetpnvv.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/godywxlco.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gapbnrfel.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gtzxosati.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/godblhfow.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdvsgzlig.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gekbjqrtb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gvmirpcym.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gemhqxtpw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gojqjhbwb.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gjxunyjsc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gjyknbhil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsedokpgw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvrjtxjh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gjwstnlwk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gtnfvduie.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gfpkmwlrr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/ghekbrmsv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gedwcceht.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gbermnhmh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gpfzsrqtc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/guszpbuzf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ghpftwauu.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ghyhnbepa.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gziyrhrjv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gfrhnomyi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gmfzciavc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/geenckqck.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gzxbuhjon.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gscdaaeur.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gxlpgbnhv.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/guzndtvtc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnrbtnmsb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/ggotsmgox.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gvrnotbbz.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/godkfgdni.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gvvovmckz.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/glkdpmzqr.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gwdpplngy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gtxzpuvxr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gwzvfcjge.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvsceyiww.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/getdxgrmr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gfuyevavh.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/geieawanq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gekeimqbl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/glaefoudk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gvxhklhhq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/ggeiquknt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gcmpvmvkv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gusdiozut.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grmewsdji.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/ggwingvsc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/giucujpah.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gydncphwt.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gccwwcvhf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/grnjapurf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/goqwopron.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gdmsedrpu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/grqofplhw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gskvlcasf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gmetzbnxk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gqfddkbtc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbikhueik.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gsbcjfdqv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gbiahblfh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gfmaklkpk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/goffxsdzr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gaskeskhn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gseqcgqbz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gvxukbfbq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gqqwqtkwm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gylsmnvgw.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gvgfmeqew.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghisqulhd.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gbzbxpvkc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gnsudvsqw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gedyimawa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gdjovvttv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gczihqrmv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gzdicywaf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gzcdybpac.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gflgozbqw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gltdeoaaq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gaimdxrjc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gytqmnxmu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gnizgujhq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gkipgyrru.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/grdsljcpu.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/guxemrxzo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gomeuuvqf.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gapevwudr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/grpshlqmo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gljsrneiy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfdtvun.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpzdjuerc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/guyjgzukg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gpixchfcu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gnrlzwcgc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gscjhscjs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gqedcfjbt.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gprxlvqrp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gjliwcwtu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gfqbsjtws.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gqfmmigvd.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gzmekafbl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/guleqbbvv.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/ghdkkkhxh.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/glzmebhjn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gbckyqqzc.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gowwyxlpo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gkdvirfcy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/goilovogo.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/ggzlezmhg.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gbtjywlyg.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/grxifziyv.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gvydyjnyj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghtaumlem.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gdeacnits.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gatpxwell.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/goiqpcbkm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gonrlrhzc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqfbtcgqp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gbdqfumes.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gftajwgxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxezcqoqu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkcwdboxe.sHtML


<!-- 参考信息 -->