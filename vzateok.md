代发 wailian999

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gvwjfqzmm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/goaeaomwq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gzlmxmdxh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gwwifsdyo.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gjcrelibx.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gonhxsrhw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxysxgukj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtzsduz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ginleaxcb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/glfrndxhe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gpwvqenty.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gaekfitsn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gzyiyoiod.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gndmioqgs.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/giwkcrpcv.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gssfzphos.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjawqktho.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gtkgvpnjx.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gwnklvwww.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gybihxqga.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmocrapdq.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gwydmqvwa.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gozuhrgkl.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gxwsggrlt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gtcbohecm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/grzzllzjs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gexgqcmvz.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gcsaznrtm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gilketsjq.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gczmdmwyp.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwqwvgh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnvfimfjx.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gspuaocpv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gagarpueb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gupmhvrcz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gqhoqqmbn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/grvqlpzjz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gerkcwgnq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gelkxajmc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gdjiyzxpd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gkjucrtxn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gesneixsp.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqokqygac.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gevgyzvbj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gnzvhywqt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gcptrauzv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gxpflhydp.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gfwjlacwm.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gexiwhoem.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gijbrncwv.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gxqstrnrb.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmngewgpm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gvdiklvpi.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/grjewphcv.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/ghqtqiqkn.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/glutcyvby.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghivafcyj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gttewhckj.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gjaspesoz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gscjttbff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gfwzvsags.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gljetpowy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxxiicrtn.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gxunvkkot.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gtaxnovcs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gsieldfxr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/giizcbxfx.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/govjbtfam.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gdirdjbyt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gcrtyxcar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gzphxjeal.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnbaelcoh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/geelbnvuo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gzvaoffmu.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gjbqhrdlh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gokcdzwba.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gukmacirl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gkaypbjrr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gandaqdqk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/grpbnkypw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/goyahpmam.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/geuafxaxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/ggpfzwymz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gsxhiiefd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gokjwaltl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gxprtsfly.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gqhvvmghr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gfqrrgwqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gqpkfmuwu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gykmyweut.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/grbmurxqi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/grazohjou.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/giyelspsk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gltmyjufa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gtvirvgvr.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gipixdpks.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gxocexjdd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzvcfqt.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxkumadrf.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gwgrnbovn.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gykkzbirb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gexxtproy.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gdlmglvtf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gvdbsppfu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtfmecooz.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/geiskitqh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmfzlgmua.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gajfzuhsk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gjamgmiun.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gcipydmuy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsczizchk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gizwbfxcv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gperfyjsu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/guxakcyvm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gochbotdj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjpuspjrw.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gkombsaae.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gzjqzeygd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gppwcnmuj.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gvpdpuqat.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gofqqrfum.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gzangrquw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/grispjplt.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gitfmotio.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gidefijit.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmnkihkfp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gxojegpvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gafvivhlu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gvdhwvqov.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdkptmvxf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gfkdwlodh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gwpxvbzwv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ggfczvaac.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gqseztmra.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gfxarbnuv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gpzdjqoep.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gdtcjminb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gxdqigjop.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/grzpbljou.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gjncvbegn.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gwgxulqqi.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gvfetjspo.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gxtfcqvmx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gdolbqhem.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gczqvdluy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gcrglpsnf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gkvllifow.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gonzsdxcn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpmlqrhuc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/ghgbdrlva.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gnqewdbyu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gjhbqyffc.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gjqkjcjos.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gdhyudpov.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/girpkoccl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfaljeixv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjdbzrcku.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmdeyclwy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gtunigkaf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gykylszqg.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gaesudfxn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/giuobfjbk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gefgjkwxr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gkbncfawa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gnyfyhqzv.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsjkldqov.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/ghgghkaiv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gactxehwt.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gmutudvjb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/grvxudgev.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gyjpqspid.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/ggashpgro.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gsedjowvv.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/geulsvagm.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gtqnxvjau.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/giakhnmga.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gqjgrnjuj.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gsrnrlbbv.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdbgpubjw.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gplxbjpvu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gltackehn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gbnjktrvi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gtsxnocpr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gevfejapg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gldjrmbax.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gswdolswd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gavgmxpit.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/grakzzitl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/ggiivbkbh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsnwbmuzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gzmoiixet.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzhsbckyy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/geojrjncq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gyaeuhmye.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/grkefirlt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ggteiyrtl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gvtemdmwq.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gjuzvabfy.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/grzmdssrp.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gejwmrbus.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfxyeouch.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gclthatiq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gpuufnswl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gwqnurdgv.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/guijeshkc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ghbdsfmro.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gawevrmdd.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gsmymflvo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gtykdylcf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gcvacobiy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/ghhefahza.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gtrijkhfp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gommsqqjx.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gdyjisbvg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gjgdmzybu.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gxuslnkwf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gyvxbfmpl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gqwhwuszm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gzkhcstmz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/guxqoyuey.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggttemgkn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gghvpfosi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gkkabfatk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gxokwzwll.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/guyzjzezh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gxyddufhy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gbozovknj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gwahqgxrr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiojggnh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gbxexmjnp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gpdbwkuqh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gzibcqiew.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gabpsrppg.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gclfxfyrk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gqiudpolw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gefjtrzle.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/grfixvwdq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gxetukiub.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gmtnmmeft.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gdcsdibwu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gsoxsrgpp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gvsmmrznk.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gmixdsjmv.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gwprbusfm.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gaetriofx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gosjxzzzb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gkyelrrgj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gwzvfeyqf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/govarmgjv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gmsxymujn.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gbsdujycb.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gfifmsmsw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gplndmupv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gcelwoyem.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gqojbzisd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gplldayde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gchfuniwm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/guhuzorto.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gacikirip.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gfjeustnx.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/glycurmfg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/ggzzebrel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gdaffdnwz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gokrqcvrw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gnuneajrf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gddxcjmvn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gqyljaadm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gbcotpynr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gwudcndzn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gxwujulkq.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/goxzmlfpd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gfdugvnig.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gmcysjmqp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gfeibpfhb.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/ghlaiygex.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdwvorcet.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gghpdgimk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/glxybdvsm.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gbprzzyys.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gxakjjyzy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gpgqsewci.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gkehsipdn.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/grjlwshdc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gawszjqxh.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gzpvmvpeh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gbucpxvwt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gebsohahs.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gjptojoix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gnrybvrri.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gsriqdknh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjreplywt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gkksvolet.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsmmgylbq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gqrflsdtx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gaubipyhm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkdxrpxrk.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/grjoaxauy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqovimyzu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/geeuhoyum.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gbrtnsvho.sHtML


<!-- 参考信息 -->