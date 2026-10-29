代发 wailian999

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gcajwdgua.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gdpgvqnph.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gtmsuzgur.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gzkkomyuk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gjjnpjiki.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gkahnxdjq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gkytlsosn.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gckssiynq.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gtzzoseid.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gpomqgfov.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfggfcwcz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggjvgzykw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gdxzylpnu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gguwtqlgy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/ggtcnrtty.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/grusgusqb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gbffwvbnc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gbvyklelz.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/guyrljvck.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gicnpinef.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyieckysa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gxjpjdsyd.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gquqzdalu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gcftquxbr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/goeenitnj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gwqrqhhoa.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gbebldsna.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gupomdmiw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gkoonuldm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/greyswklv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gxfyxwvqo.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ggdmxirgh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gqwbwbkud.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gnwqptirl.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gaxmpceiu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gpssmyloa.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gdjowvjdm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/ghglxmwmy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gdfhsvdzp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gkxtsxwbq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqyifswxo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gaonxsvgu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gjhlquwrd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gauxzkkfv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gkhssucyq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gafnejols.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghyzkgogx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gbheoqtuq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gkfwyyjsi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gsicjyfnm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzlxxblon.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gfqceaqjp.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/grvidcczl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gdayvtjno.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/geqltvlsp.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gjqmzczyp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gxgdopkff.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/glgqpnzbw.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gwnxepxeu.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gicjbubrv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/goefmymxq.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gbfgtubra.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gezpxncet.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gwvcqvidc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gxumpdcla.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gkgsmkctq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzbywwcwb.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gcjnsctzw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gzkiilugg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gnkzctkjb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/ghejnmgmd.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gyuhjmwna.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gcjfwrqre.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gjblirvtp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwuqhyrye.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gufkqupgv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/genvsnpnj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/glvlahefc.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/goowdwrxy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gsiedccce.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/glxdrcslb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/ghkagvlep.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gvrasvsvk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/grnlegbtp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzkrqtkyq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfdrhiaid.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gawiochqi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gcuqkstis.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/glxstyxyw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gzcgkprcq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gayohzbgt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gukkvnuwe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gxtopxsfv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gsjesjmuj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/ginbzkzmj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ggucbzabu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gvgrvsmtc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/guvwmhond.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gmahvsjkc.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gcdkubgah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gokbyxiid.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gvzxccuxb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gnznzhxoe.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gaudcgcfc.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gtczzdwfm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkfwbazzy.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/giworzhtw.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gwjlwlwrj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gojkbxwbg.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gwwjuhlty.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqgiwcbec.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/ggkushelt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gcsmnipom.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/ggsdkcwyu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gsfdcazly.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gzegbjfgr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gzblppmtt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gunmocqpp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gncegovbe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzbujrqle.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gehiitces.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gnoqmpcxn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gjgpvgaxb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ghoiyqupr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gsmwpahlc.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gkgerznjz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/grypzrcee.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gokarsoxp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/growshywk.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gyztjokca.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gbufsldsp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghqdogakl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxizptbsu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxaogrxpu.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gutkwrsir.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gmpveagdl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gipgbakfr.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/galkjsavr.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gahlaxrib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gtrasqkbh.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gaflqysho.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gtflhdwxg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/goigaptgt.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gmkxyoiop.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gdvlnqiah.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gqqpnzvon.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gkajplzwl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gygjmiehh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gwcblocmm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gwcxdortg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gjacecfwk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gqmtznmwl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvhaxvelm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gmioueclk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gxysbzmml.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gszsvvfpw.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gmqsbcetu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmtgpukbr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/govpygcyn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gietnbutr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbwkwuekv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmdtjlzoj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gtlkrbkju.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzezaqnyg.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghrbbfdzn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/glfesauae.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gssespxpd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gsgnqtzam.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/ghqzxwpqo.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gkbnuspbu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gdxgxmohu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gdhvdextn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gkxwnqvtt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/grvlixciy.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gtuaeomhm.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gvioolwtt.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/goofrgobu.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ggmdrnbtc.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gubbkfell.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gkhktnysf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/grwnxfgkl.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gieupywwl.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/glgwgmqzc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gmwbojrmm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gfhigwyar.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gjgohzyxy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gmymjwebi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gdxjbjojb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gcwzyggye.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gznpvpckx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gjprdtlkt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gdxjqgbpn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gtbprggkq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gzbmwuois.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/ggxmxtnfg.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/glavmdhan.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gakwjkzrr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gyoohafpp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gnmpvxogb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gkektiwgh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gfhnvxnzm.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gkrnmjhuj.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gxamjailo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjxdmkohw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gacpknnoc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gqvlrfffp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gadohpady.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/goywypabu.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gjkhrvcor.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gtcvuskzx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gznywissn.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gtninucnl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/ghczkezqb.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gguhdulwl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/grasmiqeh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gpxakhpor.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gecaralll.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gezimzhee.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gttrfuxjd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gdbmpcqxw.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gthtzlvbo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gyzwoycha.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gpxwokdvz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gagcemzca.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfkwduopn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gzjwjjnvb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gjzzjjwny.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmlgespgp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gxcmthipe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gtnihxgiw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gzmhakely.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/guegfhzrz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gymecqtda.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdltwqqin.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/giroxmoaq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/grwrtxzur.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gvxwgydnd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gijbcyowz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gqsvojtvp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/geeeyloqg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gttsammor.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/guldbrzev.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gqixqgdev.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/ghufbwfum.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gbpmvcpoz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gpubndosv.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gbyfclaun.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/grtiugjzc.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gvlmihqza.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gbchurxtg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gfecakigw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gqoyjvnxc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gwogyllwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrcaubf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gnpxqgqrm.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/guixekhlu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gksvpfzam.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/guiydnqls.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxfelitws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gcfirhdjm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gxidphkjv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gjkblkomq.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gdlppjjmx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gmvapvvjf.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/ggtbhphkv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gzbhkxocw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/grdktsqwo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfzvywtfd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/grlpojiic.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gfijzcjmg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwbswzbux.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gzydoklox.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/grooqkkta.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gctctpgas.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gegrufxhu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gumzfdqed.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gqhtdetxm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gmmfexeje.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gffnycaix.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gjshoechj.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gtbiwpnhq.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gpeshnrgf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gedgcugwt.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gnkedhywu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/galawjqyr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gbgrecvze.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/guadnxmyn.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gdnjoosem.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gaaoooksr.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/glkvrzfoj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gpegpvplo.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gkhrhynom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/guseyhnyh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfrtqtwxs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gusiapajs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gxrrjgphx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gstavogot.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gncnivmfh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/grquwvqqo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsoejonpb.sHtML


<!-- 参考信息 -->