代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gdhqdwuqg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gschojnxv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gfivuosaf.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gifnpsohv.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbfbsltif.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gmsnmbrpd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gktwhnwpp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gfkwvhsno.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gdiosteuj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gsavwzihm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/ggfpnsctu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gqkzqvicl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/getkdywvw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/ghiikjgek.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gpszweoiq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gxpirajhi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghsmtmyzo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gcbhbixyf.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gpnhmkoif.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwtmsorgd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gmyaqbqqz.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gikjezdhj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwkpsdnsg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzqywhsbs.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gfvonbrzh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gnnvqvlks.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gdbjiukiv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gycfxtzqt.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxzjmhycz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gzyolzxsj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gqquexpop.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gsnnkqdur.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gqbyzaleq.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gspfyaeuz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gagdoychs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmlazrgkx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwelsgmbo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gkwthgntw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gzcmtsbkt.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/grrkobcbf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gxsymkwix.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gcozmegnn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/ghsrmckmt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gbtxveijh.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gduqvngfq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsxzqqkcf.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gfnvlqxfy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gbqacnmjs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gmvkkresu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gjxqxsegl.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/glvupnuhc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gapnrrxyf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gqfbdimcd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/ghfwchohr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/grljyqmje.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gaulscgye.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gufdqacxh.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gdybydzhp.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gnzelqoau.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gxgujtqic.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gzzzlsxwg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gopotaone.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gsmqegojc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gmgdidofz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gwbhlkwsw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gxlliagfu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gfktukdlf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/ghbfhllsx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/givhhrfgv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gfdoqqsgq.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gtxyupera.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gbqrmufln.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gciiyedfh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gqflatfri.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gjauqzfjl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/goelfpyuv.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gxvjcwgfn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gomprobmw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgubhoc.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/glpxlyphk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/grxnbeuhf.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gtcmjucya.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghuqrqrfp.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/glcyhmdga.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyqnmyxbl.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/ggircgrtp.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gdpqufqcm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gtlsxmivk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gxhkowfkq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gcpasxxsk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/grjyywsiv.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gssabrveu.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/glfetfkgz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gsnffzldl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gcadoowvh.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gxfjhunzj.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gbpnpbepo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gssjxgbev.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfvatoeuk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gsvirvtet.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gaonhspzv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gdzrklpjf.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxzpjudsp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gkkglgrjf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gjyjbggkz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gcdvffosr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gkxtvronn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gaqrzqcvs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/girjpiicz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/geldfvvlk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdoeeshsm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/goxmiqihw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/ghzwruran.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gobufnrcn.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gavsfxuot.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gbaundvjq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gytiskjhe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxepsxuln.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gqqxrztuu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gpekwkigi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gwxmajrqk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gstetezmv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/glpanulqm.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gexutdryp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gasghjszi.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gepihynlb.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gzokozgpl.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gnvmyuxzk.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gtdcxboon.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/ghzlsvyrb.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gbfhvyzbb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gzpmszylc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gebyzticq.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwoutyrlk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnmthaauq.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/grnmqyrwe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/guxaxwmku.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gggcwngzh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gdgabbhma.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmnvvtzjn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gxyuinjqw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gbogxzgga.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gyckarujd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzhzqcogd.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gghvymyak.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gwvtniynj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gmbpirdnu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gamsrnghr.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/grhgewlqk.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gxicgjsck.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gejmmtbfw.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/ggruzwthe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gkjmwfhdy.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/grsgccbgx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gwmfbrvuf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gsgleqatn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzqbcysre.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gisasmoty.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gfoxnggra.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/glthwxrku.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/glxwrxtrm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gscqsjvuk.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gjpobubjm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/guamhrchl.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gpblclwob.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gpfvhdmtp.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/grrpztecy.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gaestcane.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gojznlyme.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gekvqawly.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gpcnzpfxs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gmaydghck.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gcptimnmg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gmvocfgvw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghaslblta.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gfrdecftt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gvmufwbix.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gdeabbyaj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/giqsqatgg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvpxfbljy.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/ggqouulxu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gggxuywmx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gaqrvgdsl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gajypwvxr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gngfspifa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gswzbioch.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gprxdddvg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkfmtpyok.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdpixsdmm.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gwfmhuhef.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gdaknlnzq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gradxvxqs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gqacxdbnp.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gdusufnap.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gafhibpqi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/getpukgfe.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gawbezvgm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gjdrekzsi.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gkokfmpxr.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gkmuedjvg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/goukvtlno.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/giwpcxkhm.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gfocjlzqv.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/goqiqylub.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gmfsnfand.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghfkujnye.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gshecdoet.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gmkawzyrc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/glvsiserr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gsdfpazio.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gqficnlyd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gvflyeqpb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gymjhgsof.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gwpumiibm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gxwkbrpvd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gwbaqwvog.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gpccwrfvt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjozscfhq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gccvdzond.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwucdnnbd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvicwxtfl.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gprylpqnb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/grciqsmdg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqlhyaofn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gjsctlvpb.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gopgmmcbl.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gudebvaqe.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/ghmyfjxtl.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gxiawkhxl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gvdpabroz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/grphvtvjo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gobgbnxyd.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gmkxxgrrc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gmcswueby.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gjlcxwigo.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmhnobarj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gfmlyuwrp.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gxshtdgzc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gszyybvta.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/guqtpmrut.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gvhusmoth.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ggbsqhvth.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gmpxtdzcb.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gaaonaxgj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gvaswsalf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gzwodthan.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gtgvgognr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ggusceaut.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gbzclstcj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gzkpymumv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gxpptxlff.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gfaszzlxv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/ggimnvnbk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gejlgxffs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gjriktziv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gojxzytja.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gddhtspkq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gwgzxqysa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gzmzxpicx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gwglvagjk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gmgfsrwjr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gsbbujgsw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gwwlqcteg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/glcmjyhtj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gwllbxtfz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gjpqnipmz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/googtdbqs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ghyyzcfjc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gacjpenzw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gwunlzkgh.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gvgvaxfsk.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gvgossxfs.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gdewiymke.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gyzimbxfj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gduifauxc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gkgkxxjzs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gpjpxopet.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghwgjstgm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/ggiaasvfc.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gukzjxoup.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gszjvycni.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gmtpoipxg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gwpbmqjqi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gjnwfvarj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gxfuowqfw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/guzxbmknh.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/goafmkbhf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gkdremcqe.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gcopzamzy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gtdztmmma.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwvjvaez.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gslrluhge.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gpxbpsnmj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gxgogwhab.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gskljojab.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gckpyfziu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gdhnhcgeo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/guoodcahw.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gyvxjexfr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjexardlm.sHtML


<!-- 参考信息 -->