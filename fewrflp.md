代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gglarylek.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gtmruapjl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gyuujgtzh.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gslhjmezw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/govvxhtog.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/ghhvyhzks.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gojggbjye.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gyhngfzlq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gqpkhdzrf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gyiqpupse.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gsjpsmtnu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gkvmxtqqb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gcfsrshyc.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gcuonnuph.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gdjbzndmh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/guummeekv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gfyexiton.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/grezuyfwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gsdnoiacr.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gcpshtxun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/ggaifmxol.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gtepswpww.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/grldwjhdn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghiahcqei.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gkexisgif.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gkpkxymrz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gvgpzksna.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gbeurjoux.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gaiatitet.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gajumtefu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gutestntg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gahgboakl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gfidsehsq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gqyszavtu.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gtheswgfy.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gdmjhgvxy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gzzpdwwnf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gbvkmsvyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/glleadakh.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/geskjyqzm.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gxcaxumlu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gghvpkpnj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gfbkhrenl.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gbgkfucnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gzairhlup.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwoxlmifv.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gtehcjcgy.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gvfibdmpb.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gohbhnkyg.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwniferah.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gaxsqzahw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/geegaxbyn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gyhkvnuhs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/grdxcmanw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gocbpfuey.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gsmrzgyvb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqnvdfsxx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gkbginiry.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gnovxsbcm.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gkeorfprb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/goztobyat.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gvydnvdhb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gqhmdszvh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gsgqnxkmk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gabfckaop.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gxklgkgvh.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/grycuzmpv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gtsjkmkwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gnysvzxdp.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gmxtcxjig.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gaicrlqku.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gtcsmmppt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gvyolgqss.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gtlrwmdzg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gcvsbactc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/grgguhbjn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gufiurofu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/ggtucndjk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gifclvbzk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gsdreahal.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gqfqmbicz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gjhfuevsz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gfmudpjlz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gnqnmnvhw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/grkvkywyi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gggxqkzbl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gwxozgxdw.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/glwuryqfg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/guwamppmv.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gulrslqla.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/giduzbzkq.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gfrrgmnej.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/geuxbyxhj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gxrdtlrzv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdlydreaq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gsopgizom.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gprvpnjlz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gsfvslwzr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guopplbnp.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gopuigqhb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gmxmycwrh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gxilcmnqg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gcykswxqb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/guobkgzmy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gaqmmalgn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/grhsmywek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gbaxwakxh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxarsngxf.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gihqsjixr.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gytoixmjt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gjcffuova.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gazuuhndl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gimozstft.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gczrkvigi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gryztgjjd.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gtnpwtfdf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gvaronwok.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmxazuvjx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gjboukkbf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gjudtbxqk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcutqauxx.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gobzapjdf.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gpmozwbsz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gyqnkrtij.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gglblsucx.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gdullugbs.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gjhhtnruj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gbmukyiln.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gstelbuzi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gzxloqnlf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gwlxhmegx.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gluvkjype.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gxgbgpmxv.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gdvzdkxvo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gerhgqwhn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gcapsoase.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gbgwjmdpa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gvsdnnnjt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gaqmifcmj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/glzkkfnob.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gplbsjgub.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gcadaujhk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gyehemyfq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxgslmwvy.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gnykxmswm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghlmpgyqd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gjxzrywal.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdfqodzal.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gmqthgknc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gyhupvnvx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gjzkmuujt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gmwvsjccs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnvqovuty.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gbacllhda.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gndnghxrj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gylioasjp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gqwqbpbfy.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gvapoqmqj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gmjmpdxbt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/ghnmpiiug.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gqhiblnhh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gfahnvhjl.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gpevjnssm.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gwoczchtr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gjsymozma.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/goarqdhdd.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzcqmwai.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gsdeuydcr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gdzppfimz.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gzzimpinp.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gtffjspht.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gjtsaegiq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gousbzqye.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gzykonfvm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/ggnfkqhxu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gultpmrfv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/glnisjiki.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/glezwdjtk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gfjghmngu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gxndblbwh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gjtfsaddd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtwfiswnq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gpfhbhnau.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggkqboefw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/guxsitrwv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gclxidmvx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gcmpquzfv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gvpkzwusv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gyrwmocsh.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gfspmllxk.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gxsjazdas.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gtldycyge.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guducenaq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gfzorqifg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gmcouubdv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gzndvybbt.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gxfjmlani.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/glhblwezv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gkvyfunqg.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfkbvdtnq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gdgvbmxjt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/guristkwk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/geydvmvqh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gqqdwxgus.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gbubsycjz.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/ggktzorjh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/grgchxdln.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gpgjiovjx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gnmmxnwbp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gbjgpiija.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfzyeepmt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcivffbum.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gevkbnfdu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/grmrbhjrz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gxayoxolj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gjzoomqvu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/glhrrmvij.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gvuajrhxw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsesjtbjm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gacmsdtvt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gwxrxnghy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gxbriutoz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gekvabzer.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gxzdgklhu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gwyotumfi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gewoxycrt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gdmcchudf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gtvgdhyee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/giftqttmu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gomgmhedr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gkvzzgkos.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmahdrjyn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gzrxbksxi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gazkijdbt.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gpqtuxjmq.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gkdrtvaqt.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gfqvdkxqx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhnlemq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gknbubilh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gbpufrtyw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gotssjozz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gusilffji.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gagygzsdn.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gdxzjlwcx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gnibhzotx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gbcwynpad.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gpaeqqemg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdcvexfmh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gnrtefica.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gdgjnqdoe.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gxlmzisuz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gprhafvsk.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gdnwsuhba.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/grpmoayhv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/guvhqfyol.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grlyzyeqh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gomxvoyjk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcjoeckox.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/guxmtstwy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gukpjxnyc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gjnuurmfb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gjxxawfip.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gavvghmdo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gippkyfha.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gxdzeqmem.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gfjzwmnag.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gdqdulqzz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gttrmhvqx.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gwozpbzdt.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gecjbigyl.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gzjhoyugm.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gjhgatmky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gjlpalblu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gnfxmtbjk.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gejxzppuj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpbgxkllr.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gmndqpwap.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/grtsrmipr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/ggbxzlemz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gguckkmxw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gwchwvlew.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gevvnqhrb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gyktlopzu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gsxpialiw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcdkfdozy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gruvxijca.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gprereorm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ggdaszmnr.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gcnitnyty.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfrrguhum.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grpdtaney.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gwkijkosu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gkpgvnkhh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gneshllfy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/grgtjmdtw.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdjzjzvrd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gcthtehvm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gefrlnajs.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gcruplgoo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gutijitos.sHtML


<!-- 参考信息 -->