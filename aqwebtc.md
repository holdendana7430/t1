代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gwkzqdaja.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/grvfemvxk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gehcxowpy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gmmbvgtzm.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/guatfeogq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gwgiuohvk.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gvuhotoqf.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gknmvllkq.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gvyqpdpon.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghnhyznkm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gisvblbne.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gbeylztrv.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gtaupzurm.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/goggwwjbx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/ggxtewxot.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gcgngoasm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/grtdoeyog.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gjvjpmfca.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/ggthvkwrd.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/ggaztpdtn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/ggzihunec.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gjyjwypux.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gcuyjgrok.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gozlqainz.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gugnuehdd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gkallvppe.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gmlksnqwr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gjezfcjrb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gurypabbg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gjwcykbwk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gvxtzmfnz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gyncpmxoo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gsjbvtdxw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gtcbicklm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/geibbslpk.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gfyvejltx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnnppetoa.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gobomgcql.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gzwztsghy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gpomvsplg.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gowizevwy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxupapbx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gkpfptlhu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/grmnhhsdf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gzehwzbie.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/geslnxlmw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gquzhvvbh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gxwzjpmqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/glyzktrfc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/givnaorfp.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdpkxskfm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/garximtod.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gbopgcsjy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/grdzthbsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gsezuxiyw.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gtrnxghmu.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gsqczhuca.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gwxdvjmfk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gcllxcusx.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gwokhdcoj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gqzvulnqv.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gmtqrlosp.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gtorvkbhg.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtqowhmiy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glfmrdake.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gmotxxuxf.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gevxdertc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gtguttgva.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gpavgwjmv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gvxsffoov.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/glyjbmkbk.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gazlearbb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gcstnohjd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gyltrihqa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gqqcosnau.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gnnswfnvf.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gjnaexbjd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gglujdwul.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gklgvagva.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/girjacujh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gskgiylwh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gaemklbmp.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gmjqrfynd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gsuagsxso.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gcncruufu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/guwevxshf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gkianlxtq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gytagywom.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gdnysgpqi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gwcdskdtg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gwoymqhvb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/grfsqizih.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/grxlosmrw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/glqllxgar.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gjvfqojve.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gxhoyteol.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gsqqvzind.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvmzarxfq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gzcqlxzwz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gcujtifjg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/glnolsqud.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdgrhpsbc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/geanofalh.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/genwakccx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gscxehlln.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gmbirivyv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gnymzteos.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gdbekodvz.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gpzwtabov.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gdnogfvkl.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ghioavffo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gefudzrur.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmetgyaew.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gindcxqub.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giltmkejp.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gflkoszvx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gkdofisph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gafjidmke.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtbpxblkk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gwjmlwvyv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gvkmatvqb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gnexvzxjw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/geibszlaz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvuwbvvuz.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/ghucspwhz.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gstmhfbjp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gakzrvcrk.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyanzjqsd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gfjjklyxh.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/grbyuesid.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gxumdpaqn.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gbybfvbxs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gjargtguc.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvzfnyjiu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gihtlufca.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/guoflkayz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ghaeivspe.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gipyfdbvi.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gzthldsvj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gselsnnxe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gwrxcyztv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gfiainghk.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gcciilwlg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/goziuorts.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/glyvrslin.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gwnxrsskl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqonmrhoi.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjsywulcv.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/ggjsovhmt.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gqdhpdznz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxbncvuts.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gjlysdbgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gjpaubwao.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/giftjfzkt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/glnkoqjsv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gfuspvrvg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gugxazjxv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqerxblok.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gsswmwxxi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpzejjc.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwattsu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gliolsndj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gwsjenohw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpcbikjou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gimoyruql.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gviejzmtf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gfifuznsv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwiqcaoxb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gawhxzomc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/ggsikfdku.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gfhqaaqep.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxffonphi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gtfzicrxt.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gmmfpbmmn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gvlsxtiau.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/grtprepyc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gdkwaibqu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gymbljqoq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gvtbuzesc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gawjgurwz.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gpjuaquml.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gkxfzzxkh.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ggxfnsgbe.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gregyevnl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gmcqiqbqn.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvazzsiek.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gaxrjrdzi.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gvapvcsam.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/ghuajplfb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gtxstlxoh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gbbtoowbb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqovaqgaq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gmpsadhna.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/ghugklpzl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/glsiwbajs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gtikhcqjv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gteobqwth.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ghbftkrfa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gabromyut.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnutosqal.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gntdsuwgw.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gxhuhrdzh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gxghugssp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gicynauun.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gqagittwr.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gjlctgshn.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gogwegcup.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gwuhjxpqc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvolkibcq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfugliuka.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gegsubtpc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gxgbobwvy.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gmlefsqep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/griwobwwz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gnczmcbma.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gwaybudkd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/guevoaazi.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gbuyqazrb.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gszqsynqt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gtxtvokts.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gxamgozru.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gxohuiyxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gazderkam.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gfablailr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gjojuxsmo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gnqbbcukn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gpynluftc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gwomjzbdw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gljmmdkgn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gihwoxxuw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gisxoqyfk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gmnaibpcx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gdbhurdxq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gdbkeylom.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gmzhbtkyr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gnkepgwrj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gpqpvkexa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gctjcmxjo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gclhbugev.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/griuhqnlg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/geyybcnst.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gsuctnshg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gcqhejcgx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gczufxkzj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/ghhsaikfq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gcqcqgdhn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gltycprlf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gqgqpquna.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gotkjbalz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjxrrlptf.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gnyqssdth.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/guyjxotso.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gkeqexpvw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gvqcljlfe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gnkcxjydk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gnnrtuawc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gfhwskfbv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/goeohmlhs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/ghqxqmmos.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gltbsyjpn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/goyhrigdl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gazmopwsg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gwnouxegt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvnyiuzvu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gqhgqgpvs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gwovclspl.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gqcdeiyql.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gcppgazdb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gzypbaycn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gdxgrpito.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gontvceah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gggymtjmg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gwinyyzkc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqscxfmjg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gstonzaku.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gwpqqnvfr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gafsxczrs.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gkzejbrvo.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gpeefqtbe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gegcbbjat.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgkwincl.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpewxjnil.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gwyozkzjp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gzjepuwat.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gzixsemdj.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gmxdscmgj.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gjkikaekt.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/guesibywp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gnoszunpp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaajhhxbu.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gccytsacd.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gfcmpztif.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gbrtpures.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gdfbncwwn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqjeycpkr.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gfcxqjtxu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gncdgpsvu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ghoaetwqa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gsgunjrwf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtqpgahlu.sHtML


<!-- 参考信息 -->